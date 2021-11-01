#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-black
PKG_VERSION:=21.9b0
PKG_RELEASE:=1

PYPI_NAME:=black
PKG_HASH:=7de4cfc7eb6b710de325712d40125689101d21d25283eed7e9998722cf10eb91

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-black
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=The uncompromising code formatter.
  URL:=https://pypi.org/project/black/
  DEPENDS:= 
endef

define Package/python3-ha-black/description
 Black makes code review faster by producing the smallest diffs possible.
endef

$(eval $(call Py3Package,python3-ha-black))
$(eval $(call BuildPackage,python3-ha-black))
