#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-numpy
PKG_VERSION:=1.21.1
PKG_RELEASE:=$(AUTORELEASE)

PYPI_NAME:=numpy
PKG_HASH:=dff4af63638afcc57a3dfb9e4b26d434a7a602d225b42d746ea7fe2edf1342fd

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE.txt
PKG_CPE_ID:=cpe:/a:numpy:numpy

PKG_CONFIG_DEPENDS:= \
        CONFIG_NUMPY_OPENBLAS_SUPPORT

# yes, zip... sigh
PYPI_SOURCE_EXT:=zip
HOST_PYTHON3_PACKAGE_BUILD_DEPENDS:=Cython

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

PYTHON3_PKG_SETUP_GLOBAL_ARGS += \
	build_ext \
	--fcompiler=none


define Package/python3-ha-numpy
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=The fundamental package for scientific
  URL:=https://www.numpy.org/
  DEPENDS:=+python3 \
 	   +NUMPY_OPENBLAS_SUPPORT:openblas
endef

# We need to duplicate the omitted arhitectures same as openblas
define Package/python3-ha-numpy/config
menu "Configuration"
depends on !powerpc
depends on !arc

config NUMPY_OPENBLAS_SUPPORT
        bool "Enable OpenBLAS support"
        default n

endmenu
endef

ifdef CONFIG_NUMPY_OPENBLAS_SUPPORT
define Build/Prepare/numpy-sitecfg
	echo "[DEFAULT]"                                 >  $(PKG_BUILD_DIR)/site.cfg
	echo "library_dirs = $(STAGING_DIR)/usr/lib"     >> $(PKG_BUILD_DIR)/site.cfg
	echo "include_dirs = $(STAGING_DIR)/usr/include" >> $(PKG_BUILD_DIR)/site.cfg
	echo                                             >> $(PKG_BUILD_DIR)/site.cfg
	echo "[openblas]"                                >> $(PKG_BUILD_DIR)/site.cfg
	echo "libraries = openblas"                      >> $(PKG_BUILD_DIR)/site.cfg
	echo "runtime_library_dirs = /usr/lib"           >> $(PKG_BUILD_DIR)/site.cfg
endef
endif

define Build/Prepare
	$(call Build/Prepare/Default)
	$(call Build/Prepare/numpy-sitecfg)
endef

define Package/python3-numpy/description
NumPy is the fundamental package for array computing with Python.

By default, this package is built without some modules.
For some modules to be available, the INSTALL_GFORTRAN symbol needs
to be enabled in the OpenWrt core/toolchain.
endef

$(eval $(call Py3Package,python3-ha-numpy))
$(eval $(call BuildPackage,python3-ha-numpy))