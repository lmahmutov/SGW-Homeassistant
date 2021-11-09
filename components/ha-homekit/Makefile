# SPDX-License-Identifier: GPL-2.0-only

include $(TOPDIR)/rules.mk

PKG_NAME:=ha-homekit
PKG_VERSION:=0.0.1
PKG_RELEASE:=5

PKG_SOURCE:=
PKG_SOURCE_URL:=
PKG_HASH:=unknown

include $(INCLUDE_DIR)/package.mk

define Package/ha-homekit
  CATEGORY:=Homeassistant
  SUBMENU:=Components
  TITLE:=HomeKit (metapackage)
  URL:=https://www.home-assistant.io/integrations/homekit
  PKG_DEFAULT_DEPENDS:= \
	+python3-light \
	+python3-ha-aiohomekit \
	+python3-ha-base36 \
	+python3-ha-fnvhash \
	+python3-ha-ffmpeg \
	+python3-ha-pyhap \
	+python3-ha-pyqrcode \
	+python3-ha-pyturbojpeg
endef

define Package/ha-homekit/description
  Metapackage of integration HomeKit.
endef

Build/Prepare:=:
Build/Configure:=:
Build/Compile:=:

define Package/ha-homekit/install
	true
endef

$(eval $(call BuildPackage,ha-homekit))
