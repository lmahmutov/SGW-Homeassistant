#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-httpx
PKG_VERSION:=0.23.0
PKG_RELEASE:=1

PYPI_NAME:=httpx
PKG_HASH:=f28eac771ec9eb4866d3fb4ab65abd42d38c424739e80c08d8d20570de60b0ef

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-httpx
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=(HA CORE) HTTPX - HTTP client for Python.
  URL:=https://pypi.org/project/httpx/
  DEPENDS:= \
	+python3-ha-certifi \
	+python3-ha-httpcore \
	+python3-ha-rfc3986 \
	+python3-ha-sniffio
endef

define Package/python3-ha-httpx/description
 HTTPX is a fully featured HTTP client for Python 3, which provides sync
 and async APIs, and support for both HTTP/1.1 and HTTP/2.
endef

$(eval $(call Py3Package,python3-ha-httpx))
$(eval $(call BuildPackage,python3-ha-httpx))
