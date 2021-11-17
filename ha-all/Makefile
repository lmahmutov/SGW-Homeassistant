# SPDX-License-Identifier: GPL-2.0-only

include $(TOPDIR)/rules.mk

PKG_NAME:=ha-all
PKG_VERSION:=0.1
PKG_RELEASE:=1

PKG_SOURCE:=
PKG_SOURCE_URL:=
PKG_HASH:=unknown

include $(INCLUDE_DIR)/package.mk

define Package/ha-all
  CATEGORY:=Homeassistant
  TITLE:=HA with all packages (metapackage)
  PKG_DEFAULT_DEPENDS:= \
	+homeassistant \
	+ha-aioesphomeapi \
	+ha-homekit \
	+hass-configurator \
	+ha-wled \
	+ha-zha \
	+ha-ble-monitor \
	+ha-miio \
	+ha-yeelight
endef

define Package/ha-all/description
 ha-all.
endef

Build/Prepare:=:
Build/Configure:=:
Build/Compile:=:

define Package/ha-all/install
	true
endef

$(eval $(call BuildPackage,ha-all))
