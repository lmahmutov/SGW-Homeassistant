#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-zigpy-deconz
PKG_VERSION:=0.13.0
PKG_RELEASE:=1

PYPI_NAME:=zigpy-deconz
PKG_HASH:=4fd70d5eb1411ab0c9a5d74f3036c5ac5039f1c0c0d88cd231210740d961eadd

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-zigpy-deconz
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Deconz radios for zigpy.
  URL:=https://pypi.org/project/zigpy-deconz/
  DEPENDS:= +python3-light
endef

define Package/python3-ha-zigpy-deconz/description
 zigpy-deconz is a Python 3 implementation for the Zigpy project to implement deCONZ based Zigbee radio devices.
endef

$(eval $(call Py3Package,python3-ha-zigpy-deconz))
$(eval $(call BuildPackage,python3-ha-zigpy-deconz))