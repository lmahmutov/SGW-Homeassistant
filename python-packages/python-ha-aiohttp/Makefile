#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=aiohttp
PKG_VERSION:=3.7.4.post0
PKG_RELEASE:=1

PYPI_NAME:=$(PKG_NAME)
PKG_HASH:=493d3299ebe5f5a7c66b9819eacdcfbbaaf1a8e84911ddffcdc48888497afecf

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=LICENSE
PKG_CPE_ID:=cpe:/a:aio-libs_project:aiohttp

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-aiohttp
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=(HA CORE) Async http client/server framework
  URL:=https://github.com/aio-libs/aiohttp
  DEPENDS:= \
	+python3-light \
	+python3-ha-attrs \
	+python3-ha-chardet \
	+python3-ha-multidict \
	+python3-ha-async-timeout \
	+python3-ha-yarl \
	+python3-logging \
	+python3-codecs \
	+python3-cgi \
	+python3-openssl \
	+python3-ha-typing-extensions
endef

define Package/python3-ha-aiohttp/description
  Asynchronous HTTP client/server framework for asyncio and Python3.
endef

$(eval $(call Py3Package,python3-ha-aiohttp))
$(eval $(call BuildPackage,python3-ha-aiohttp))