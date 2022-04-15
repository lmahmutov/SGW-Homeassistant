#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-yeelight
PKG_VERSION:=0.7.10
PKG_RELEASE:=1

PYPI_NAME:=yeelight
PKG_HASH:=0b0e1b2be58b3524a31f51d28610d2a6e459b74ea6770bd7cfd1c8a4622c64a3

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-yeelight
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=YeeLight RGB bulbs
  URL:=https://pypi.org/project/yeelight/
  DEPENDS:=  \
	+python3-light
endef

define Package/python3-ha-yeelight/description
 A Python library for controlling YeeLight RGB bulbs.
endef

$(eval $(call Py3Package,python3-ha-yeelight))
$(eval $(call BuildPackage,python3-ha-yeelight))
