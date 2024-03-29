#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pyparsing
PKG_VERSION:=2.4.7
PKG_RELEASE:=2

PYPI_NAME:=pyparsing
PKG_HASH:=c203ec8783bf771a155b207279b9bccb8dea02d8f0c9e5f8ead507bc3246ecc1

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pyparsing
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Library for constructing grammar directly in python
  URL:=https://github.com/pyparsing/pyparsing/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-pyparsing/description
  The pyparsing module is an alternative approach to creating
  and executing simple grammars, vs. the traditional lex/yacc
  approach, or the use of regular expressions.
  The pyparsing module provides a library of classes that
  client code uses to construct the grammar directly in Python code.
endef

$(eval $(call Py3Package,python3-ha-pyparsing))
$(eval $(call BuildPackage,python3-ha-pyparsing))
