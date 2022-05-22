# SPDX-License-Identifier: GPL-2.0-only

include $(TOPDIR)/rules.mk

PKG_NAME:=ha-ble-monitor
PKG_RELEASE:=1

PKG_SOURCE_URL:=https://github.com/custom-components/ble_monitor.git
PKG_MIRROR_HASH:=7877e2301da1094c01585ec5decb3c4c903553f3d9bf3f8eae8adc4788ec223c
PKG_SOURCE_PROTO:=git
PKG_SOURCE_DATE:=2022-05-19
PKG_SOURCE_VERSION:=03bb891e05da5867401eb9bf8bcd55bfa3adef57

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
	+python3-ha-aioblescan \
	+python3-ha-btsocket \
	+python3-ha-pyric
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