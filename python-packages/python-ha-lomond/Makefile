#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-lomond
PKG_VERSION:=0.3.3
PKG_RELEASE:=1

PYPI_NAME:=lomond
PKG_HASH:=427936596b144b4ec387ead99aac1560b77c8a78107d3d49415d3abbe79acbd3

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-lomond
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Websocket Client Library
  URL:=https://pypi.org/project/lomond/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-lomond/description
 Websocket Client Library
endef

$(eval $(call Py3Package,python3-ha-lomond))
$(eval $(call BuildPackage,python3-ha-lomond))
