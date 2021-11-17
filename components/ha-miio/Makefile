# SPDX-License-Identifier: GPL-2.0-only

include $(TOPDIR)/rules.mk

PKG_NAME:=ha-miio
PKG_VERSION:=0.1
PKG_RELEASE:=1

PKG_SOURCE:=
PKG_SOURCE_URL:=
PKG_HASH:=unknown

include $(INCLUDE_DIR)/package.mk

define Package/ha-miio
  CATEGORY:=Homeassistant
  SUBMENU:=Components
  TITLE:=HA xiaomi-miio (metapackage)
  PKG_DEFAULT_DEPENDS:= \
	+homeassistant \
	+python3-ha-python-miio \
	+python3-ha-appdirs \
	+python3-ha-construct \
	+python3-ha-croniter \
	+python3-ha-natsort \
	+python3-ha-tqdm \
	+python3-ha-micloud
endef

define Package/ha-miio/description
 Passive BLE Monitor integration.
endef

Build/Prepare:=:
Build/Configure:=:
Build/Compile:=:

define Package/ha-miio/install
	true
endef

$(eval $(call BuildPackage,ha-miio))
