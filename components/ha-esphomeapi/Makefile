#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=ha-aioesphomeapi
PKG_VERSION:=9.1.1
PKG_RELEASE:=1

PYPI_NAME:=aioesphomeapi
PKG_HASH:=5f21094936be0391e385e71a39f106bc9d41ddd54d114cbab2577af8aa74f9a7

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-aioesphomeapi
  CATEGORY:=Homeassistant
  SUBMENU:=Components
  TITLE:=Python API for interacting with ESPHome devices.
  URL:=https://pypi.org/project/aioesphomeapi/
  DEPENDS:= \
      +python3-light
endef

define Package/python3-ha-aioesphomeapi/description
 Esphomeapi allows you to interact with devices flashed with ESPHome.
endef

$(eval $(call Py3Package,python3-ha-aioesphomeapi))
$(eval $(call BuildPackage,python3-ha-aioesphomeapi))
