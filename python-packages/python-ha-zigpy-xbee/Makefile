#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-zigpy-xbee
PKG_VERSION:=0.14.0
PKG_RELEASE:=1

PYPI_NAME:=zigpy-xbee
PKG_HASH:=04d06d3c5e5b2748eee93c9ac9a67fc77ded900d9f4a57a09a65023ca882406e

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-zigpy-xbee
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=XBee radios for zigpy.
  URL:=https://pypi.org/project/zigpy-xbee/
  DEPENDS:= +python3-light
endef

define Package/python3-ha-zigpy-xbee/description
 zigpy-xbee is a Python implementation for the Zigpy project to implement XBee based Zigbee radio devices from Digi.
endef

$(eval $(call Py3Package,python3-ha-zigpy-xbee))
$(eval $(call BuildPackage,python3-ha-zigpy-xbee))
