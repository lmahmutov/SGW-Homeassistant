# SPDX-License-Identifier: GPL-2.0-only

include $(TOPDIR)/rules.mk

PKG_NAME:=ha-yandexstation
PKG_RELEASE:=1

PKG_SOURCE_URL:=https://github.com/AlexxIT/YandexStation.git
PKG_MIRROR_HASH:=13fdc9b403fc1d2413216cd2db87caded0fa16f9459dac7d7294be55117e6d3b
PKG_SOURCE_PROTO:=git
PKG_SOURCE_DATE:=2022-05-14
PKG_SOURCE_VERSION:=b0eb377b8a607b5c529962c7413ea32e8e1c73e9

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(INCLUDE_DIR)/package.mk

define Package/ha-yandexstation
  CATEGORY:=Homeassistant
  SUBMENU:=Components
  TITLE:=HA YandexStation component (metapackage)
  PKG_DEFAULT_DEPENDS:= \
	+homeassistant
endef

define Package/ha-yandexstation/description
 Яндекс.Станция для Home Assistant.
endef

define Build/Prepare
        $(Build/Prepare/Default)
	$(PKG_UNPACK)
endef

define Package/ha-yandexstation/install
	$(INSTALL_DIR) $(1)/etc/homeassistant/custom_components/
	$(CP) $(PKG_BUILD_DIR)/custom_components/yandex_station $(1)/etc/homeassistant/custom_components/
endef

Build/Configure:=:
Build/Compile:=:

$(eval $(call BuildPackage,ha-yandexstation))