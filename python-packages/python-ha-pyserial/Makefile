#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pyserial
PKG_VERSION:=3.5
PKG_RELEASE:=1

PYPI_NAME:=pyserial
PKG_HASH:=3c77e014170dfffbd816e6ffc205e9842efb10be9f58ec16d3e8675b4925cddb

PKG_LICENSE:=BSD
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pyserial
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=python3-pyserial
  URL:=https://github.com/pyserial/pyserial
  DEPENDS:=+python3-light
endef

define Package/python3-ha-pyserial/description
This module encapsulates the access for the serial port. It provides backends
for Python running on Windows, OSX, Linux, BSD (possibly any POSIX compliant
system) and IronPython. The module named "serial" automatically selects the
appropriate backend.
endef

$(eval $(call Py3Package,python3-ha-pyserial))
$(eval $(call BuildPackage,python3-ha-pyserial))
