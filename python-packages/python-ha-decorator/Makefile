#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-decorator
PKG_VERSION:=4.4.2
PKG_RELEASE:=1
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_CPE_ID:=cpe:/a:python:decorator

PYPI_NAME:=decorator
PKG_HASH:=e3a62f0520172440ca0dcc823749319382e377f37f140a0b99ef45fecb84bfe7

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-decorator
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  URL:=https://github.com/micheles/decorator
  TITLE:=python3-decodator
  DEPENDS:=+python3-light
endef

$(eval $(call Py3Package,python3-ha-decorator))
$(eval $(call BuildPackage,python3-ha-decorator))
