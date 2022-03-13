#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-btsocket
PKG_VERSION:=0.2.0
PKG_RELEASE:=1

PYPI_NAME:=btsocket
PKG_HASH:=6862250b7e0973d2beea9e49d3b5ced324d80e5003a0350856879e537ba777a8

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-btsocket
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Python library for BlueZ
  URL:=https://pypi.org/project/btsocket/
  DEPENDS:=  \
	+python3-light
endef

define Package/python3-ha-btsocket/description
 Python library for BlueZ Bluetooth Management API.
endef

$(eval $(call Py3Package,python3-ha-btsocket))
$(eval $(call BuildPackage,python3-ha-btsocket))
