#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=hass-nabucasa
PKG_VERSION:=0.50.0
PKG_RELEASE:=1

PYPI_NAME:=hass-nabucasa
PKG_HASH:=24a6556f5508394909dacf0e5c3caffe4fbe7dd9c995ec5d9e26c76b5fd75f26

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/hass-nabucasa
  CATEGORY:=Homeassistant
  SUBMENU:=Components
  TITLE:=Home Assistant cloud
  URL:=https://pypi.org/project/hass-nabucasa/
  DEPENDS:= \
	+homeassistant \
	+python3-ha-acme \
	+python3-ha-aiohttp \
	+python3-ha-atomicwrites \
	+python3-ha-attrs \
	+python3-ha-cryptography \
	+python3-ha-pycognito \
	+python3-ha-pytz \
	+python3-ha-snitun
endef

define Package/hass-nabucasa/description
 Home Assistant cloud integration by Nabu Casa, Inc.
endef

$(eval $(call Py3Package,hass-nabucasa))
$(eval $(call BuildPackage,hass-nabucasa))
