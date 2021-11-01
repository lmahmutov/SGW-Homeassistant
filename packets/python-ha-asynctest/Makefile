#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-asynctest
PKG_VERSION:=0.13.0
PKG_RELEASE:=1

PYPI_NAME:=asynctest
PKG_HASH:=c27862842d15d83e6a34eb0b2866c323880eb3a75e4485b079ea11748fd77fac

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-asynctest
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Enhance the standard unittest package.
  URL:=https://pypi.org/project/asynctest/
  DEPENDS:= 
endef

define Package/python3-ha-asynctest/description
  The package asynctest is built on top of the standard unittest
 module and cuts down boilerplate code when testing libraries for asyncio.
 Currently, asynctest targets the “selector” model, hence, some features 
 will not (yet?) work with Windows’ proactor.
endef

$(eval $(call Py3Package,python3-ha-asynctest))
$(eval $(call BuildPackage,python3-ha-asynctest))
