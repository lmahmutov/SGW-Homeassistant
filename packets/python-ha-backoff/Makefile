#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-backoff
PKG_VERSION:=1.11.1
PKG_RELEASE:=1

PYPI_NAME:=backoff
PKG_HASH:=ccb962a2378418c667b3c979b504fdeb7d9e0d29c0579e3b13b86467177728cb

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-backoff
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Function decoration for backoff and retry.
  URL:=https://pypi.org/project/backoff/
  DEPENDS:= 
endef

define Package/python3-ha-backoff/description
 Decorators support both regular functions for 
 synchronous code and asyncio’s coroutines for asynchronous code..
endef

$(eval $(call Py3Package,python3-ha-backoff))
$(eval $(call BuildPackage,python3-ha-backoff))
