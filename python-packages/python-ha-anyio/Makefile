#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-anyio
PKG_VERSION:=3.6.1
PKG_RELEASE:=1

PYPI_NAME:=anyio
PKG_HASH:=413adf95f93886e442aea925f3ee43baa5a765a64a0f52c6081894f9992fdd0b

PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-anyio
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Python-anyio.
  URL:=https://pypi.org/project/anyio/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-anyio/description
 High level compatibility layer for multiple asynchronous event loop implementations.
endef

$(eval $(call Py3Package,python3-ha-anyio))
$(eval $(call BuildPackage,python3-ha-anyio))
