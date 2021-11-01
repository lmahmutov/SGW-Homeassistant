#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-aresponses
PKG_VERSION:=2.1.4
PKG_RELEASE:=1

PYPI_NAME:=aresponses
PKG_HASH:=39674af90700f1bfe2c7c9049cd8116f5c10d34d2e2427fd744b88d9e8644c94

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-aresponses
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=an asyncio testing server.
  URL:=https://pypi.org/project/aresponses/
  DEPENDS:= \
	+python3-ha-aiohttp \
	+python3-ha-pytest-asyncio
endef

define Package/python3-ha-aresponses/description
  Asyncio response mocking. Similar to the responses library used for 'requests'.
endef

$(eval $(call Py3Package,python3-ha-aresponses))
$(eval $(call BuildPackage,python3-ha-aresponses))
