# SPDX-License-Identifier: GPL-2.0-only

include $(TOPDIR)/rules.mk

PKG_NAME:=ha-zha
PKG_VERSION:=0.0.1
PKG_RELEASE:=1

PKG_SOURCE:=
PKG_SOURCE_URL:=
PKG_HASH:=unknown

include $(INCLUDE_DIR)/package.mk

define Package/ha-zha
  CATEGORY:=Homeassistant
  SUBMENU:=Components
  TITLE:=ZHA (metapackage)
  URL:=https://www.home-assistant.io/integrations/zha/
  PKG_DEFAULT_DEPENDS:= \
	+homeassistant \
	+python3-ha-bellows \
	+python3-ha-zha-quirks \
	+python3-ha-zigpy-cc \
	+python3-ha-zigpy-znp \
	+python3-ha-zigpy-zigate \
	+python3-ha-zigpy-xbee \
	+python3-ha-zigpy-deconz \
	+python3-ha-crccheck
endef

define Package/ha-zha/description
 The ZHA (Zigbee Home Automation) integration allows
 you to connect many off-the-shelf Zigbee based devices
 directly to Home Assistant, using one of the many available Zigbee coordinators.
endef

Build/Prepare:=:
Build/Configure:=:
Build/Compile:=:

define Package/ha-zha/install
	true
endef

$(eval $(call BuildPackage,ha-zha))
