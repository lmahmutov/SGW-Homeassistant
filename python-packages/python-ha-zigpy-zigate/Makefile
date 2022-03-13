#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-zigpy-zigate
PKG_VERSION:=0.8.0
PKG_RELEASE:=1

PYPI_NAME:=zigpy-zigate
PKG_HASH:=08691bb97e52dca114ace4edcbee0146f27e7c04d23a8b1b77a8450585ce2176

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-zigpy-zigate
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=ZiGate radios for zigpy.
  URL:=https://pypi.org/project/zigpy-zigate/
  DEPENDS:= +python3-light \
	+python3-ha-pyusb \
	+python3-ha-rpi-gpio
endef

define Package/python3-ha-zigpy-zigate/description
 zigpy-zigate is a Python 3 implementation for the Zigpy project to implement ZiGate based Zigbee radio devices.
endef

$(eval $(call Py3Package,python3-ha-zigpy-zigate))
$(eval $(call BuildPackage,python3-ha-zigpy-zigate))
