#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-queueman
PKG_VERSION:=0.5
PKG_RELEASE:=1

PYPI_NAME:=queueman
PKG_HASH:=ce2928b8ce07f3f4675876342d1cd3335328c5ac2a9a00df92dc5818bc2ed1d7

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-queueman
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=No project description provided.
  URL:=https://pypi.org/project/queueman/
  DEPENDS:= +python3-light 
endef

define Package/python3-ha-queueman/description
 WIP.
endef

$(eval $(call Py3Package,python3-ha-queueman))
$(eval $(call BuildPackage,python3-ha-queueman))
