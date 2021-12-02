# SPDX-License-Identifier: GPL-2.0-only

include $(TOPDIR)/rules.mk

PKG_NAME:=ha-dataplicity
PKG_RELEASE:=1

PKG_SOURCE_URL:=https://github.com/AlexxIT/Dataplicity.git
PKG_MIRROR_HASH:=9f264c8edc0ae3c7ed07f9342388025743e03a685a72c57fac9272874dbec065
PKG_SOURCE_PROTO:=git
PKG_SOURCE_DATE:=2021-07-28
PKG_SOURCE_VERSION:=6205c81a2fbbd36eddd5fc530a46a44acaf8a761

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(INCLUDE_DIR)/package.mk

define Package/ha-dataplicity
  CATEGORY:=Homeassistant
  SUBMENU:=Components
  TITLE:=HA dataplicity (metapackage)
  PKG_DEFAULT_DEPENDS:= \
	+homeassistant \
	+python3-ha-dataplicity \
	+python3-ha-six \
	+python3-ha-lomond
endef

define Package/ha-dataplicity/description
 Passive BLE Monitor integration.
endef

define Build/Prepare
        $(Build/Prepare/Default)
	$(PKG_UNPACK)
endef

define Package/ha-dataplicity/install
	$(INSTALL_DIR) $(1)/etc/homeassistant/custom_components/
	$(CP) $(PKG_BUILD_DIR)/custom_components/dataplicity $(1)/etc/homeassistant/custom_components/
endef

Build/Configure:=:
Build/Compile:=:

$(eval $(call BuildPackage,ha-dataplicity))