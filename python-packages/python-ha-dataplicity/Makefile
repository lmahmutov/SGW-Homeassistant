#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-dataplicity
PKG_VERSION:=0.4.40
PKG_RELEASE:=1

PYPI_NAME:=dataplicity
PKG_HASH:=04a53ddb2f8c83e13001bf6bf3c0cc9d0aa5342865f567556fd23171947ce034

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-dataplicity
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Platform for connected devices
  URL:=https://pypi.org/project/dataplicity/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-dataplicity/description
 Platform for connected devices
endef

$(eval $(call Py3Package,python3-ha-dataplicity))
$(eval $(call BuildPackage,python3-ha-dataplicity))
