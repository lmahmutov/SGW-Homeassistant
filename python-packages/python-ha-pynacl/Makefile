#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-pynacl
PKG_VERSION:=1.5.0
PKG_RELEASE:=1

PYPI_NAME:=PyNaCl
PKG_HASH:=8ac7448f09ab85811607bdd21ec2464495ac8b7c66d146bf545b0f08fb9220ba

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=LICENSE

PKG_BUILD_DEPENDS:=libffi/host

HOST_PYTHON3_PACKAGE_BUILD_DEPENDS:=cffi  # cffi>=1.4.1

PYTHON3_PKG_SETUP_VARS:= SODIUM_INSTALL=system

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pynacl
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Python binding to the libsodium library
  URL:=https://github.com/pyca/pynacl/
  DEPENDS:=+libsodium +python3-light +python3-ha-cffi +python3-ha-six
endef

define Package/python3-ha-pynacl/description
  PyNaCl is a Python binding to libsodium, which is a fork of the Networking and Cryptography library.
endef

$(eval $(call Py3Package,python3-ha-pynacl))
$(eval $(call BuildPackage,python3-ha-pynacl))
