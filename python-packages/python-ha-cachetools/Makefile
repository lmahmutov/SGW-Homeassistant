#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-cachetools
PKG_VERSION:=5.0.0
PKG_RELEASE:=1

PYPI_NAME:=cachetools
PKG_HASH:=486471dfa8799eb7ec503a8059e263db000cdda20075ce5e48903087f79d5fd6

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-cachetools
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Extensible memoizing collections and decorators
  URL:=https://pypi.org/project/cachetools/
  DEPENDS:= +python3-light 
endef

define Package/python3-ha-cachetools/description
Extensible memoizing collections and decorators.
endef

$(eval $(call Py3Package,python3-ha-cachetools))
$(eval $(call BuildPackage,python3-ha-cachetools))
