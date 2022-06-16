#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=ha-aioesphomeapi
PKG_VERSION:=10.10.0
PKG_RELEASE:=1

PYPI_NAME:=aioesphomeapi
PKG_HASH:=b8d801378471db0f5c39e1239e83d68fc4fd43489732c32b54ca4ddc72995215

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/ha-aioesphomeapi
  CATEGORY:=Homeassistant
  SUBMENU:=Components
  TITLE:=API for interacting with ESPHome devices.
  URL:=https://pypi.org/project/aioesphomeapi/
  DEPENDS:= +homeassistant \
	+python3-ha-protobuf \
	+python3-ha-noiseprotocol
endef

define Package/ha-aioesphomeapi/description
 Esphomeapi allows you to interact with devices flashed with ESPHome.
endef

$(eval $(call Py3Package,ha-aioesphomeapi))
$(eval $(call BuildPackage,ha-aioesphomeapi))
