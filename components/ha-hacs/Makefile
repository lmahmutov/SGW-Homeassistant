# SPDX-License-Identifier: GPL-2.0-only

include $(TOPDIR)/rules.mk

PKG_NAME:=ha-hacs
PKG_VERSION:=1.15.2
PKG_RELEASE:=1

PKG_SOURCE:=
PKG_SOURCE_URL:=
PKG_HASH:=unknown

include $(INCLUDE_DIR)/package.mk

define Package/ha-hacs
  CATEGORY:=Homeassistant
  SUBMENU:=Components
  TITLE:=HACS (metapackage)
  URL:=https://github.com/hacs/integration
  PKG_DEFAULT_DEPENDS:= \
	+python3-ha-aiofiles \
	+python3-ha-aiogithubapi \
	+python3-ha-aiohttp \
	+python3-ha-aresponses \
	+python3-ha-asynctest \
	+python3-ha-attrs \
	+python3-ha-awesomeversion \
	+python3-ha-backoff \
	+python3-ha-bellybutton \
	+python3-ha-colorlog \
	+python3-hacs-frontend \
	+python3-ha-pre-commit \
	+python3-ha-pygithub \
	+python3-ha-pytest \
	+python3-ha-pytest-asyncio \
	+python3-ha-pytest-cov \
	+python3-ha-pytest-socket \
	+python3-ha-queueman \
	+python3-ha-requests \
	+python3-ha-vulture
endef

define Package/ha-hacs/description
 HACS is a integration that gives the user a 
 powerful UI to handle downloads of custom integrations and plugins.
endef

Build/Prepare:=:
Build/Configure:=:
Build/Compile:=:

define Package/ha-hacs/install
	true
endef

$(eval $(call BuildPackage,ha-hacs))
