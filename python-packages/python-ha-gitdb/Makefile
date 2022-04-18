#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-gitdb
PKG_VERSION:=4.0.9
PKG_RELEASE:=1

PYPI_NAME:=gitdb
PKG_HASH:=bac2fd45c0a1c9cf619e63a90d62bdc63892ef92387424b855792a6cabe789aa

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-gitdb
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:= Git Object Database
  URL:=https://pypi.org/project/gitdb/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-gitdb/description
  Git Object Database.
endef

$(eval $(call Py3Package,python3-ha-gitdb))
$(eval $(call BuildPackage,python3-ha-gitdb))
