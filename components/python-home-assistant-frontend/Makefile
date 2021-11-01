#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-home-assistant-frontend
PKG_VERSION:=20211007.1
PKG_RELEASE:=1

PYPI_NAME:=home-assistant-frontend
PKG_HASH:=c2c0cd2f0ce1a701f9bf07474568591a5ba68c533cfd2fa45cfae86c3f95a44f

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

define Package/python3-home-assistant-frontend/description
 The Home Assistant frontend.
endef

$(eval $(call Py3Package,python3-home-assistant-frontend))
$(eval $(call BuildPackage,python3-home-assistant-frontend))
