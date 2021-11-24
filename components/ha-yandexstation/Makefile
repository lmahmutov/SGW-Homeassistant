# SPDX-License-Identifier: GPL-2.0-only

include $(TOPDIR)/rules.mk

PKG_NAME:=ha-yandexstation
PKG_RELEASE:=1

PKG_SOURCE_URL:=https://github.com/AlexxIT/YandexStation.git
PKG_MIRROR_HASH:=b5eec29d7159ffa9e6fcb3afc9c9149616cbad6bbd7bb18a00b39459b297dc60
PKG_SOURCE_PROTO:=git
PKG_SOURCE_DATE:=2021-10-16
PKG_SOURCE_VERSION:=abc19e2d341dc8ff5e7b5b9362592e98e413cfd1

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