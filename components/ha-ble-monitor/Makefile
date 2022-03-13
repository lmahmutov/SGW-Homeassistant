# SPDX-License-Identifier: GPL-2.0-only

include $(TOPDIR)/rules.mk

PKG_NAME:=ha-ble-monitor
PKG_RELEASE:=1

PKG_SOURCE_URL:=https://github.com/custom-components/ble_monitor.git
PKG_MIRROR_HASH:=19d9a04179870ba791d4d413e2975eafa5db6f386382e38df94b3ede449f942d
PKG_SOURCE_PROTO:=git
PKG_SOURCE_DATE:=2022-03-11
PKG_SOURCE_VERSION:=d36df5c51edd63c60921f90907d4e2c92cf1efa5

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
	+python3-ha-btsocket
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