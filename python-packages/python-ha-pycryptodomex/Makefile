#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pycryptodomex
PKG_VERSION:=3.11.0
PKG_RELEASE:=1

PYPI_NAME:=pycryptodomex
PKG_HASH:=0398366656bb55ebdb1d1d493a7175fc48ade449283086db254ac44c7d318d6d

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=COPYING

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pycryptodomex
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Cryptographic library for Python
  URL:=https://pypi.org/project/pycryptodomex/
  DEPENDS:= \
	  +python3-light
endef

define Package/python3-ha-pycryptodomex/description
  Cryptographic library for Python
endef

$(eval $(call Py3Package,python3-ha-pycryptodomex))
$(eval $(call BuildPackage,python3-ha-pycryptodomex))
