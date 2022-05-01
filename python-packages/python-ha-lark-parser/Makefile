#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-lark-parser
PKG_VERSION:=0.7.8
PKG_RELEASE:=1

PYPI_NAME:=lark-parser
PKG_HASH:=26215ebb157e6fb2ee74319aa4445b9f3b7e456e26be215ce19fdaaa901c20a4

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-lark-parser
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=a modern parsing library.
  URL:=https://pypi.org/project/lark-parser/
  DEPENDS:= \
	+python3-light
endef

define Package/python3-ha-lark-parser/description
 Lark is a parsing toolkit for Python, built with a focus on ergonomics,
 performance and modularity.
endef

$(eval $(call Py3Package,python3-ha-lark-parser))
$(eval $(call BuildPackage,python3-ha-lark-parser))
