#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-vulture
PKG_VERSION:=2.3
PKG_RELEASE:=1

PYPI_NAME:=vulture
PKG_HASH:=03d5a62bcbe9ceb9a9b0575f42d71a2d414070229f2e6f95fa6e7c71aaaed967

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-vulture
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Find dead code.
  URL:=https://pypi.org/project/vulture/
  DEPENDS:= 
endef

define Package/python3-ha-vulture/description
 Vulture finds unused code in Python programs. 
 This is useful for cleaning up and finding errors in large code bases.
endef

$(eval $(call Py3Package,python3-ha-vulture))
$(eval $(call BuildPackage,python3-ha-vulture))
