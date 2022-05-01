#
# Copyright (C) 2015, 2017-2018 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-six
PKG_VERSION:=1.16.0
PKG_RELEASE:=1

PYPI_NAME:=six
PKG_HASH:=1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

HOST_BUILD_DEPENDS:=python3/host

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/host-build.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk


define Package/python3-ha-six
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Python 2 and 3 compatibility library
  URL:=https://github.com/benjaminp/six
  DEPENDS:=+python3-light
endef

define Package/python3-ha-six/description
Six is a Python 2 and 3 compatibility library.  It provides utility functions
for smoothing over the differences between the Python versions with the goal of
writing Python code that is compatible on both Python versions.  See the
documentation for more information on what is provided.
endef

define Host/Compile
	$(call HostPython3/ModSetup,,install --prefix="" --root="$(STAGING_DIR_HOSTPKG)")
endef

Host/Install:=

$(eval $(call HostBuild))

$(eval $(call Py3Package,python3-ha-six))
$(eval $(call BuildPackage,python3-ha-six))
