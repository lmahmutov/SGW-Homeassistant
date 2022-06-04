#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-async-upnp-client
PKG_VERSION:=0.30.1
PKG_RELEASE:=1

PYPI_NAME:=async_upnp_client
PKG_HASH:=36a70e531112aa9ebe8df025a066b764c0915af8dfaab08b235d29ca900ffa78

PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-async-upnp-client
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Async UPnP Client
  URL:=https://pypi.org/project/async-upnp-client/
  DEPENDS:= \
	+python3-ha-aiohttp \
	+python3-ha-async-timeout \
	+python3-ha-defusedxml \
	+python3-ha-didl-lite \
	+python3-ha-voluptuous
endef

define Package/python3-ha-async-upnp-client/description
  Asyncio UPnP Client library for Python/asyncio.
endef

$(eval $(call Py3Package,python3-ha-async-upnp-client))
$(eval $(call BuildPackage,python3-ha-async-upnp-client))
