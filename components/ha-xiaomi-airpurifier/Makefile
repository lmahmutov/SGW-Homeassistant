# SPDX-License-Identifier: GPL-2.0-only

include $(TOPDIR)/rules.mk

PKG_NAME:=ha-xiaomi-airpurifier
PKG_RELEASE:=1

PKG_SOURCE_URL:=https://github.com/syssi/xiaomi_airpurifier.git
PKG_MIRROR_HASH:=9cee977fe40dd37d6dc4dfe68bc78b318c848556527a7e162dd546cf9753bbb1
PKG_SOURCE_PROTO:=git
PKG_SOURCE_DATE:=2022-03-12
PKG_SOURCE_VERSION:=b5ef2b05dd385a3e58503c4d774d5982811cf391

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(INCLUDE_DIR)/package.mk

define Package/ha-xiaomi-airpurifier
  CATEGORY:=Homeassistant
  SUBMENU:=Components
  TITLE:=HA xiaomi-airpurifier (metapackage)
  PKG_DEFAULT_DEPENDS:= \
	+homeassistant \
	+python3-ha-python-miio
endef

define Package/ha-xiaomi-airpurifier/description
 Xiaomi Mi Air Purifier & Xiaomi Mi Air Humidifier.
endef

define Build/Prepare
        $(Build/Prepare/Default)
	$(PKG_UNPACK)
endef

define Package/ha-xiaomi-airpurifier/install
	$(INSTALL_DIR) $(1)/etc/homeassistant/custom_components/
	$(CP) $(PKG_BUILD_DIR)/custom_components/xiaomi_miio_airpurifier $(1)/etc/homeassistant/custom_components/
endef

Build/Configure:=:
Build/Compile:=:

$(eval $(call BuildPackage,ha-xiaomi-airpurifier))