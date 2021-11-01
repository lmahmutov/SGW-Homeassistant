#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-rpi-gpio
PKG_VERSION:=0.7.0
PKG_RELEASE:=1

PYPI_NAME:=RPi.GPIO
PKG_HASH:=7424bc6c205466764f30f666c18187a0824077daf20b295c42f08aea2cb87d3f

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-rpi-gpio
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=A module to control Raspberry Pi GPIO channels.
  URL:=https://pypi.org/project/rpi-gpio/
  DEPENDS:= +python3-light
endef

PYTHON3_PKG_SETUP_ARGS:=

define Package/python3-ha-rpi-gpio/description
 This package provides a class to control the GPIO on a Raspberry Pi.
endef

$(eval $(call Py3Package,python3-ha-rpi-gpio))
$(eval $(call BuildPackage,python3-ha-rpi-gpio))
