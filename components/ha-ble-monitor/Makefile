# SPDX-License-Identifier: GPL-2.0-only

include $(TOPDIR)/rules.mk

PKG_NAME:=ha-ble-monitor
PKG_VERSION:=0.1
PKG_RELEASE:=1

PKG_SOURCE:=
PKG_SOURCE_URL:=
PKG_HASH:=unknown

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

Build/Prepare:=:
Build/Configure:=:
Build/Compile:=:

define Package/ha-ble-monitor/install
	true
endef

$(eval $(call BuildPackage,ha-ble-monitor))
