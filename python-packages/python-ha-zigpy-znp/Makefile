#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-zigpy-znp
PKG_VERSION:=0.7.0
PKG_RELEASE:=1

PYPI_NAME:=zigpy-znp
PKG_HASH:=efaf473e780ef61013aa287cdca91f7e04c559eea88ae6b9e566fdb91abc7535

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-zigpy-znp
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=A library for zigpy TI ZNP radios.
  URL:=https://pypi.org/project/zigpy-znp/
  DEPENDS:= \
	+python3-ha-jsonschema \
	+python3-ha-coloredlogs
endef

define Package/python3-ha-zigpy-znp/description
 zigpy-znp is a Python library that adds support for
 common Texas Instruments ZNP (Zigbee Network Processors)
 Zigbee radio modules to zigpy, a Python Zigbee stack project.
endef

$(eval $(call Py3Package,python3-ha-zigpy-znp))
$(eval $(call BuildPackage,python3-ha-zigpy-znp))
