#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-hacs-frontend
PKG_VERSION:=20220401183545
PKG_RELEASE:=1

PYPI_NAME:=hacs-frontend
PKG_HASH:=ddb49b67bb088d6a6b691e5adcb1b30b9a250f68f3bfcdf862ee281c038f1ce8

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-hacs-frontend
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=The HACS frontend
  URL:=https://pypi.org/project/hacs-frontend/
  DEPENDS:= +python3-light 
endef

define Package/python3-hacs-frontend/description
 The HACS frontend system.
endef

$(eval $(call Py3Package,python3-hacs-frontend))
$(eval $(call BuildPackage,python3-hacs-frontend))
