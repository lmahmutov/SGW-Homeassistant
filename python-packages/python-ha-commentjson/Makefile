#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-commentjson
PKG_VERSION:=0.9.0
PKG_RELEASE:=1

PYPI_NAME:=commentjson
PKG_HASH:=42f9f231d97d93aff3286a4dc0de39bfd91ae823d1d9eba9fa901fe0c7113dd4

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-commentjson
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=JavaScript style comments in JSON files.
  URL:=https://pypi.org/project/commentjson/
  DEPENDS:= \
	+python3-ha-lark-parser
endef

define Package/python3-ha-commentjson/description
 commentjson (Comment JSON) is a Python package that helps you create
 JSON files with Python and JavaScript style inline comments.
 Its API is very similar to the Python standard library’s json module..
endef

$(eval $(call Py3Package,python3-ha-commentjson))
$(eval $(call BuildPackage,python3-ha-commentjson))
