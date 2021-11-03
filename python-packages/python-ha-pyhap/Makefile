#
# Copyright (C) 2021 @lmahmutov
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pyhap
PKG_VERSION:=4.1.0
PKG_RELEASE:=1

PYPI_NAME:=HAP-python
PKG_HASH:=d26a6830f1078b64f4e981ce8039462a7c7c5b9851ecc79309bb2f45cc7e98aa

PKG_LICENSE:=Apache-2.0
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pyhap
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=HomeKit Accessory Protocol implementation in python.
  URL:=https://pypi.org/project/HAP-python/
  DEPENDS:= \
	+python3-ha-cryptography \
	+python3-ha-h11 \
	+python3-ha-zeroconf
endef

define Package/python3-ha-pyhap/description
 HomeKit Accessory Protocol implementation in python 3. With this project,
 you can integrate your own smart devices and add them to your iOS Home app.
 Since Siri is integrated with the Home app, you can start voice-control your
 accessories right away.
endef

$(eval $(call Py3Package,python3-ha-pyhap))
$(eval $(call BuildPackage,python3-ha-pyhap))
