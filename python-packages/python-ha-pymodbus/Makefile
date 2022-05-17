#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pymodbus
PKG_VERSION:=2.5.3
PKG_RELEASE:=1
PKG_LICENSE:=BSD-2-Clause

PYPI_NAME:=pymodbus
PKG_HASH:=5ef68c1a109bdb467c830ef003ef2db6494349a5248e4af946fe21c9eefe7e74
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pymodbus
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=A fully featured modbus protocol stack in python
  URL:=https://pypi.org/project/pymodbus
  DEPENDS:= \
	+python3 \
	+python3-ha-six
endef

define Build/Prepare
	$(Build/Prepare/Default)
	$(CP) ./files/* $(PKG_BUILD_DIR)/
endef

define Package/python3-ha-pymodbus/description
  Pymodbus aims to be a fully implemented modbus protocol stack implemented using
  twisted/asyncio/tornado. Its orignal goal was to allow simulation of thousands
  of modbus devices on a single machine for monitoring software testing.
endef

$(eval $(call Py3Package,python3-ha-pymodbus))
$(eval $(call BuildPackage,python3-ha-pymodbus))
