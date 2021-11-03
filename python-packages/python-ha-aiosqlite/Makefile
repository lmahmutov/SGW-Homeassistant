#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-aiosqlite
PKG_VERSION:=0.17.0
PKG_RELEASE:=1

PYPI_NAME:=aiosqlite
PKG_HASH:=f0e6acc24bc4864149267ac82fb46dfb3be4455f99fe21df82609cc6e6baee51

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-aiosqlite
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=asyncio bridge to the standard sqlite3 module.
  URL:=https://pypi.org/project/aiosqlite/
  DEPENDS:= +python3-light
endef

PYTHON3_PKG_SETUP_ARGS:=

define Package/python3-ha-aiosqlite/description
 It replicates the standard sqlite3 module,
 but with async versions of all the standard connection and cursor methods,
 plus context managers for automatically closing connections and cursors.
endef

$(eval $(call Py3Package,python3-ha-aiosqlite))
$(eval $(call BuildPackage,python3-ha-aiosqlite))
