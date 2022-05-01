#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-ciso8601
PKG_VERSION:=2.2.0
PKG_RELEASE:=1

PYPI_NAME:=ciso8601
PKG_HASH:=14ad817ed31a698372d42afa81b0173d71cd1d0b48b7499a2da2a01dcc8695e6

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE.txt

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-ciso8601
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=(HA CORE) Fast ISO8601 date time parser for Python
  URL:=https://github.com/closeio/ciso8601
  DEPENDS:=+python3-light
endef

define Package/python3-ha-ciso8601/description
  ciso8601 converts ISO 8601 or RFC 3339 date time strings into Python datetime objects.
endef

$(eval $(call Py3Package,python3-ha-ciso8601))
$(eval $(call BuildPackage,python3-ha-ciso8601))


