# SPDX-License-Identifier: GPL-2.0-only

include $(TOPDIR)/rules.mk

PKG_NAME:=ha-webrtc
PKG_RELEASE:=1

PKG_SOURCE_URL:=https://github.com/AlexxIT/WebRTC.git
PKG_MIRROR_HASH:=982bcaef41c4853cdd86370addf59eee8dc62ededf1ad3a31a49b78dfda5879f
PKG_SOURCE_PROTO:=git
PKG_SOURCE_DATE:=2022-05-15
PKG_SOURCE_VERSION:=3e1099d65cf66ac7b7e1bcc787722f48f25c6bea

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(INCLUDE_DIR)/package.mk

define Package/ha-webrtc
  CATEGORY:=Homeassistant
  SUBMENU:=Components
  TITLE:=HA WebRTC Camera component (metapackage)
  PKG_DEFAULT_DEPENDS:= \
	+homeassistant
endef

define Package/ha-webrtc/description
 Home Assistant custom component for viewing IP cameras RTSP stream in real time using WebRTC and MSE technology.
endef

define Build/Prepare
        $(Build/Prepare/Default)
	$(PKG_UNPACK)
endef

define Package/ha-webrtc/install
	$(INSTALL_DIR) $(1)/etc/homeassistant/custom_components/
	$(CP) $(PKG_BUILD_DIR)/custom_components/webrtc $(1)/etc/homeassistant/custom_components/
endef

Build/Configure:=:
Build/Compile:=:

$(eval $(call BuildPackage,ha-webrtc))