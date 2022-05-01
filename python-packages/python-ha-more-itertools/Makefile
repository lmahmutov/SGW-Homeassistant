#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-more-itertools
PKG_VERSION:=8.6.0
PKG_RELEASE:=1

PYPI_NAME:=more-itertools
PKG_HASH:=b3a9005928e5bed54076e6e549c792b306fddfe72b2d1d22dd63d42d5d3899cf

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-more-itertools
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=More routines for operating on iterables, beyond itertools
  URL:=https://github.com/erikrose/more-itertools
  DEPENDS:=+python3-light
endef

define Package/python3-ha-more-itertools/description
  more-itertools library collects additional building blocks,
  recipes, and routines for working with Python iterables.
endef

$(eval $(call Py3Package,python3-ha-more-itertools))
$(eval $(call BuildPackage,python3-ha-more-itertools))
