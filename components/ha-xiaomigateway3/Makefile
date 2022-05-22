# SPDX-License-Identifier: GPL-2.0-only

include $(TOPDIR)/rules.mk

PKG_NAME:=ha-xiaomigateway3
PKG_RELEASE:=1

PKG_SOURCE_URL:=https://github.com/AlexxIT/XiaomiGateway3.git
PKG_MIRROR_HASH:=0eb80da8660dd5af2c1def11bd5da2c9182b19f996117afc9f38438c7e1af1c0
PKG_SOURCE_PROTO:=git
PKG_SOURCE_DATE:=2022-05-15
PKG_SOURCE_VERSION:=7dc5849510a1fd940500da35d77bcfc36ce831fd

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(INCLUDE_DIR)/package.mk

define Package/ha-xiaomigateway3
  CATEGORY:=Homeassistant
  SUBMENU:=Components
  TITLE:=HA Xiaomi Gateway 3 component (metapackage)
  PKG_DEFAULT_DEPENDS:= \
	+homeassistant
endef

define Package/ha-xiaomigateway3/description
 Xiaomi Gateway 3 for Home Assistant.
endef

define Build/Prepare
        $(Build/Prepare/Default)
	$(PKG_UNPACK)
endef

define Package/ha-xiaomigateway3/install
	$(INSTALL_DIR) $(1)/etc/homeassistant/custom_components/
	$(CP) $(PKG_BUILD_DIR)/custom_components/xiaomi_gateway3 $(1)/etc/homeassistant/custom_components/
endef

Build/Configure:=:
Build/Compile:=:

$(eval $(call BuildPackage,ha-xiaomigateway3))