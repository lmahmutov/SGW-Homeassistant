#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-websocket-client
PKG_VERSION:=0.58.0
PKG_RELEASE:=3

PYPI_NAME:=websocket_client
PKG_HASH:=63509b41d158ae5b7f67eb4ad20fecbb4eee99434e73e140354dc3ff8e09716f

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-websocket-client
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=WebSocket client for Python. hybi13 is supported
  URL:=https://github.com/websocket-client/websocket-client
  DEPENDS:= \
	+python3-light \
	+python3-logging \
	+python3-openssl \
	+python3-ha-six
endef

define Package/python3-ha-websocket-client/description
  websocket-client module is WebSocket client for python. This provide the low
  level APIs for WebSocket. All APIs are the synchronous functions.

  websocket-client supports only hybi-13.
endef

$(eval $(call Py3Package,python3-ha-websocket-client))
$(eval $(call BuildPackage,python3-ha-websocket-client))
