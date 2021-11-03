#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-base36
PKG_VERSION:=0.1.1
PKG_RELEASE:=1

PYPI_NAME:=base36
PKG_HASH:=6f221783c5499bd5fd4a1102054df9638d6232ff5ca850c21fd1efe5070c1a96

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-base36
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=homeassistant.components.homekit
  URL:=https://pypi.org/project/base36/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-base36/description
Yet another implementation for the positional numeral system using 36 as the radix.
endef

$(eval $(call Py3Package,python3-ha-base36))
$(eval $(call BuildPackage,python3-ha-base36))
