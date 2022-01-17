#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-home-assistant-frontend
PKG_VERSION:=20211229.1
PKG_RELEASE:=1

PYPI_NAME:=home-assistant-frontend
PKG_HASH:=82556327d88e9a1008183eb93c742ef65ed673f96be574726b69a2db4fd4560b

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
	$(call Build/Prepare/Default)
	$(FIND) $(PKG_BUILD_DIR)/hass_frontend/frontend_es5 -name '*.js' -delete
	$(FIND) $(PKG_BUILD_DIR)/hass_frontend/frontend_es5 -name '*.map'  -delete
	$(FIND) $(PKG_BUILD_DIR)/hass_frontend/frontend_es5 -name '*.txt' -delete
	$(FIND) $(PKG_BUILD_DIR)/hass_frontend/frontend_latest -name '*.js' -delete
	$(FIND) $(PKG_BUILD_DIR)/hass_frontend/frontend_latest -name '*.map' -delete
	$(FIND) $(PKG_BUILD_DIR)/hass_frontend/frontend_latest -name '*.txt' -delete

	$(FIND) $(PKG_BUILD_DIR)/hass_frontend/static/mdi -name '*.json' -maxdepth 1  -delete
	$(FIND) $(PKG_BUILD_DIR)/hass_frontend/static/polyfills -name '*.js' -maxdepth 1 -delete
	$(FIND) $(PKG_BUILD_DIR)/hass_frontend/static/polyfills -name '*.map' -maxdepth 1 -delete

	# shopping list and calendar missing gzipped
	gzip $(PKG_BUILD_DIR)/hass_frontend/static/translations/shopping_list/*

	$(FIND) $(PKG_BUILD_DIR)/hass_frontend/static/translations -name '*.json' -delete
endef


define Package/python3-home-assistant-frontend/description
 The Home Assistant frontend.
endef

$(eval $(call Py3Package,python3-home-assistant-frontend))
$(eval $(call BuildPackage,python3-home-assistant-frontend))
