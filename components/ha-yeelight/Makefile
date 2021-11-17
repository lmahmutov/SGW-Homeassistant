# SPDX-License-Identifier: GPL-2.0-only

include $(TOPDIR)/rules.mk

PKG_NAME:=ha-yeelight
PKG_VERSION:=0.1
PKG_RELEASE:=1

PKG_SOURCE:=
PKG_SOURCE_URL:=
PKG_HASH:=unknown

include $(INCLUDE_DIR)/package.mk

define Package/ha-yeelight
  CATEGORY:=Homeassistant
  SUBMENU:=Components
  TITLE:=HA yeelight (metapackage)
  PKG_DEFAULT_DEPENDS:= \
	+homeassistant \
	+python3-ha-yeelight \
	+python3-ha-yeelightsunflower \
	+python3-ha-future
endef

define Package/ha-yeelight/description
 Passive BLE Monitor integration.
endef

Build/Prepare:=:
Build/Configure:=:
Build/Compile:=:

define Package/ha-yeelight/install
	true
endef

$(eval $(call BuildPackage,ha-yeelight))
