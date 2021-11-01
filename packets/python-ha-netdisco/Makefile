#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-netdisco
PKG_VERSION:=2.9.0
PKG_RELEASE:=2

PYPI_NAME:=netdisco
PKG_HASH:=3a92c533ed199a18202754ae2e848efaa58b70a7294bae6c77bbb6ce4ccfcace

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=LICENSE.md

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-netdisco
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Discover devices on your local network
  URL:=https://github.com/home-assistant/netdisco
  DEPENDS:= \
	  +python3-light \
	  +python3-ha-requests \
	  +python3-ha-zeroconf
endef

define Package/python3-ha-netdisco/description
  NetDisco is a Python 3 library to discover local devices and services.
  It allows to scan on demand or offer a service that will scan the network in the background in a set interval.
endef

$(eval $(call Py3Package,python3-ha-netdisco))
$(eval $(call BuildPackage,python3-ha-netdisco))

