#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python3-ha-hatasmota
PKG_VERSION:=0.5.1
PKG_RELEASE:=1

PYPI_NAME:=HATasmota
PKG_HASH:=933b13485ac2d32c4d90f77314d300bd27bbc1c8be28bdead6be72650f7f9287

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0 MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-hatasmota
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=parse and construct Tasmota MQTT messages
  URL:=https://pypi.org/project/hatasmota/
  DEPENDS:= \
	+python3-setuptools
endef

define Package/python3-ha-hatasmota/description
   Python module to help parse and construct Tasmota MQTT messages.
endef

$(eval $(call Py3Package,python3-ha-hatasmota))
$(eval $(call BuildPackage,python3-ha-hatasmota))
