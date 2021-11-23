# SPDX-License-Identifier: GPL-2.0-only

include $(TOPDIR)/rules.mk

PKG_NAME:=ha-ble-monitor
PKG_RELEASE:=1

PKG_SOURCE_URL:=https://github.com/custom-components/ble_monitor.git
PKG_MIRROR_HASH:=9f264c8edc0ae3c7ed07f9342388025743e03a685a72c57fac9272874dbec065
PKG_SOURCE_PROTO:=git
PKG_SOURCE_DATE:=2021-11-18
PKG_SOURCE_VERSION:=0913e5fb1ccb47a3ff6850f3c86ebb698228ceac

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(INCLUDE_DIR)/package.mk

define Package/ha-ble-monitor
  CATEGORY:=Homeassistant
  SUBMENU:=Components
  TITLE:=HA ble-monitor (metapackage)
  PKG_DEFAULT_DEPENDS:= \
	+homeassistant \
	+python3-ha-pycryptodomex \
	+python3-ha-janus \
	+python3-ha-aioblescan
endef

define Package/ha-ble-monitor/description
 Passive BLE Monitor integration.
endef

define Build/Prepare
        $(Build/Prepare/Default)
	$(PKG_UNPACK)
endef

define Package/ha-ble-monitor/install
	$(INSTALL_DIR) $(1)/etc/homeassistant/custom_components/
	$(CP) $(PKG_BUILD_DIR)/custom_components/ble_monitor $(1)/etc/homeassistant/custom_components/
endef

Build/Configure:=:
Build/Compile:=:

$(eval $(call BuildPackage,ha-ble-monitor))