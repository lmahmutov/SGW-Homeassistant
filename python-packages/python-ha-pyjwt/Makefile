#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=pyjwt
PKG_VERSION:=2.3.0
PKG_RELEASE:=1

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

PYPI_NAME:=PyJWT
PKG_HASH:=b888b4d56f06f6dcd777210c334e69c737be74755d3e5e9ee3fe67dc18a0ee41

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pyjwt
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=(HA CORE) JSON Web Token implementation in Python
  URL:=http://github.com/jpadilla/pyjwt
  DEPENDS:=+python3
endef

define Package/python3-ha-pyjwt/description
  A Python implementation of RFC 7519.
endef

$(eval $(call Py3Package,python3-ha-pyjwt))
$(eval $(call BuildPackage,python3-ha-pyjwt))
