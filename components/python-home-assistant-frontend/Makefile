#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python3-home-assistant-frontend
PKG_VERSION:=20220601.0
PKG_RELEASE:=1

PYPI_NAME:=home_assistant_frontend
PKG_SOURCE:=$(PYPI_NAME)-$(PKG_VERSION)-py3-none-any.whl
PKG_SOURCE_URL:=https://github.com/home-assistant/frontend/releases/download/$(PKG_VERSION)/
PKG_HASH:=58644a26ae36f5f23165027354adb116a5d436b2186c28ebdb34d2ce90656a42
UNPACK_CMD=ar -p "$(DL_DIR)/$(PKG_SOURCE)" | unzip -q "$(DL_DIR)/$(PKG_SOURCE)" -d $(1)

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-home-assistant-frontend
  CATEGORY:=Homeassistant
  SUBMENU:=Components
  TITLE:=Home Assistant frontend
  URL:=https://pypi.org/project/home-assistant-frontend/
  DEPENDS:= \
	+python3-light  \
	+python3-ha-tzdata
endef

define Build/Prepare
	$(Build/Prepare/Default)
	$(CP) ./files/* $(PKG_BUILD_DIR)/
	$(FIND) $(PKG_BUILD_DIR)/hass_frontend/frontend_es5 -name '*.js' -delete
	$(FIND) $(PKG_BUILD_DIR)/hass_frontend/frontend_es5 -name '*.map'  -delete
	$(FIND) $(PKG_BUILD_DIR)/hass_frontend/frontend_es5 -name '*.txt' -delete
	$(FIND) $(PKG_BUILD_DIR)/hass_frontend/frontend_latest -name '*.js' -delete
	$(FIND) $(PKG_BUILD_DIR)/hass_frontend/frontend_latest -name '*.map' -delete
	$(FIND) $(PKG_BUILD_DIR)/hass_frontend/frontend_latest -name '*.txt' -delete

	$(FIND) $(PKG_BUILD_DIR)/hass_frontend/static/mdi -name '*.json' -maxdepth 1  -delete
	$(FIND) $(PKG_BUILD_DIR)/hass_frontend/static/polyfills -name '*.js' -maxdepth 1 -delete
	$(FIND) $(PKG_BUILD_DIR)/hass_frontend/static/polyfills -name '*.map' -maxdepth 1 -delete
	#update version
	$(SED) 's/Version: .*/Version: $(PKG_VERSION)/' $(PKG_BUILD_DIR)/PKG-INFO
	$(SED) 's/version = .*/version = $(PKG_VERSION)/' $(PKG_BUILD_DIR)/setup.cfg
	# shopping list and calendar missing gzipped
	gzip $(PKG_BUILD_DIR)/hass_frontend/static/translations/shopping_list/*

	$(FIND) $(PKG_BUILD_DIR)/hass_frontend/static/translations -name '*.json' -delete
endef

define Package/python3-home-assistant-frontend/description
 The Home Assistant frontend.
endef

$(eval $(call Py3Package,python3-home-assistant-frontend))
$(eval $(call BuildPackage,python3-home-assistant-frontend))
