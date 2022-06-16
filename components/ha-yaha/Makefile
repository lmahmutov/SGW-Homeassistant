# SPDX-License-Identifier: GPL-2.0-only

include $(TOPDIR)/rules.mk

PKG_NAME:=ha-yaha
PKG_RELEASE:=1

PKG_SOURCE_URL:=https://github.com/dmitry-k/yandex_smart_home.git
PKG_MIRROR_HASH:=a6f4a87428ab8dc022b787c2c66c86adf5c8ef6af52589397b7dfef051298d94
PKG_SOURCE_PROTO:=git
PKG_SOURCE_DATE:=2022-05-28
PKG_SOURCE_VERSION:=5dc5b2dca6a1c1ff3f8ae87690c01a5d59bd3776

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(INCLUDE_DIR)/package.mk

define Package/ha-yaha
  CATEGORY:=Homeassistant
  SUBMENU:=Components
  TITLE:=Yandex Smart Home component (metapackage)
  PKG_DEFAULT_DEPENDS:= \
	+homeassistant
endef

define Package/ha-yaha/description
 Yandex Smart Home for HomeAssistant.
endef

define Build/Prepare
        $(Build/Prepare/Default)
	$(PKG_UNPACK)
endef

define Package/ha-yaha/install
	$(INSTALL_DIR) $(1)/etc/homeassistant/custom_components/
	$(CP) $(PKG_BUILD_DIR)/custom_components/yandex_smart_home $(1)/etc/homeassistant/custom_components/
endef

Build/Configure:=:
Build/Compile:=:

$(eval $(call BuildPackage,ha-yaha))