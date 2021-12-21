#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-aiosignal
PKG_VERSION:=1.2.0
PKG_RELEASE:=1

PYPI_NAME:=aiosignal
PKG_HASH:=78ed67db6c7b7ced4f98e495e572106d5c432a93e1ddd1bf475e1dc05f5b7df2

PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-aiosignal
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Python-aiosignal.
  URL:=https://pypi.org/project/aiosignal/
  DEPENDS:=+python3-light \
	+python3-ha-frozenlist
endef

define Package/python3-ha-aiosignal/description
 aiosignal: a list of registered asynchronous callbacks.
endef

$(eval $(call Py3Package,python3-ha-aiosignal))
$(eval $(call BuildPackage,python3-ha-aiosignal))
