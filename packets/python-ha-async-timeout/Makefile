#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=async-timeout
PKG_VERSION:=3.0.1
PKG_RELEASE:=2

PYPI_NAME:=async_timeout
PYPI_SOURCE_NAME:=async-timeout
PKG_HASH:=0c3c816a028d47f659d6ff5c745cb2acf1f966da1fe5c19c77a70282b25f4c5f

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-async-timeout
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=(HA CORE) Timeout context manager
  URL:=https://github.com/aio-libs/async-timeout
  DEPENDS:= \
	+python3-light \
	+python3-asyncio
endef

define Package/python3-ha-async-timeout/description
Timeout context manager for asyncio programs
endef

$(eval $(call Py3Package,python3-ha-async-timeout))
$(eval $(call BuildPackage,python3-ha-async-timeout))