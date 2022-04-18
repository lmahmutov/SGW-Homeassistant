# SPDX-License-Identifier: GPL-2.0-only

include $(TOPDIR)/rules.mk

PKG_NAME:=ha-yandexstation
PKG_RELEASE:=1

PKG_SOURCE_URL:=https://github.com/AlexxIT/YandexStation.git
PKG_MIRROR_HASH:=0eb80da8660dd5af2c1def11bd5da2c9182b19f996117afc9f38438c7e1af1c0
PKG_SOURCE_PROTO:=git
PKG_SOURCE_DATE:=2022-02-18
PKG_SOURCE_VERSION:=20f04529969d50fdfd9ba0eab58c7e88a25ccb8d

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