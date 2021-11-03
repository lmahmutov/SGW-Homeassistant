#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-aiohomekit
PKG_VERSION:=0.6.2
PKG_RELEASE:=1

PYPI_NAME:=aiohomekit
PKG_HASH:=1ba9356f44c7f13b0bedbcd6c49fa8c2e5df3936b1a5442cd87b59b8fdefb2f0

PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-aiohomekit
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=HomeKit protocol for controlling Homekit
  URL:=https://pypi.org/project/aiohomekit/
  DEPENDS:= \
	+python3-ha-commentjson \
	+python3-ha-cryptography \
	+python3-ha-zeroconf
endef

define Package/python3-ha-aiohomekit/description
 This library implements the HomeKit protocol for controlling Homekit
 accessories using asyncio.
 .
 It's primary use is for with Home Assistant. We target the same versions
 of python as them and try to follow their code standards.
endef

$(eval $(call Py3Package,python3-ha-aiohomekit))
$(eval $(call BuildPackage,python3-ha-aiohomekit))
