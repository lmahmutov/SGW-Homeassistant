#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-ply
PKG_VERSION:=3.11
PKG_RELEASE:=2

PYPI_NAME:=ply
PKG_HASH:=00c7c1aaa88358b9c765b6d3000c6eec0ba42abca5351b095321aef446081da3

PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=README.md
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-ply
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=lex and yacc for Python
  URL:=http://www.dabeaz.com/ply/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-ply/description
PLY is a 100% Python implementation of the common parsing tools lex
and yacc.
endef

$(eval $(call Py3Package,python3-ha-ply))
$(eval $(call BuildPackage,python3-ha-ply))
