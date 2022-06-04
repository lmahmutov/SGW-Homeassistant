#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-cryptodome
PKG_VERSION:=3.14.1
PKG_RELEASE:=1

PYPI_NAME:=pycryptodome
PKG_HASH:=e04e40a7f8c1669195536a37979dd87da2c32dbdc73d6fe35f0077b0c17c803b

PKG_LICENSE:=BSD-2-Clause
PKG_LICENSE_FILES:=LICENSE.rst
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_CPE_ID:=cpe:/a:pycryptodome:pycryptodome

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

PYTHON3_PKG_SETUP_ARGS:=
PYTHON3_PKG_SETUP_VARS:= \
  CONFIG_BIG_ENDIAN="$(CONFIG_BIG_ENDIAN)"

define Package/python3-ha-cryptodome
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=A self-contained cryptographic library for Python
  URL:=https://www.pycryptodome.org/
  DEPENDS:=+libgmp +python3
  PROVIDES:=python3-crypto
endef

define Package/python3-ha-cryptodome/description
PyCryptodome is a self-contained Python package of low-level
cryptographic primitives.
endef

$(eval $(call Py3Package,python3-ha-cryptodome))
$(eval $(call BuildPackage,python3-ha-cryptodome))
