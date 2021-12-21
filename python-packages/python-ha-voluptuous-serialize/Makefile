#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=ha-voluptuous-serialize
PKG_VERSION:=2.5.0
PKG_RELEASE:=1

PYPI_NAME:=voluptuous-serialize
PKG_HASH:=5359f2e0a4f972ae03066e0777b4f0755c9226b2af099ca4fc55432efd1a447b

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=COPYING

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-voluptuous-serialize
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=(HA CORE) Python Voluptuous Serialize
  URL:=https://github.com/balloob/voluptuous-serialize
  DEPENDS:= \
	+python3-light \
	+python3-ha-voluptuous
endef

define Package/python3-ha-voluptuous-serialize/description
  Convert Voluptuous schemas to dictionaries so they can be serialized.
endef

$(eval $(call Py3Package,python3-ha-voluptuous-serialize))
$(eval $(call BuildPackage,python3-ha-voluptuous-serialize))
