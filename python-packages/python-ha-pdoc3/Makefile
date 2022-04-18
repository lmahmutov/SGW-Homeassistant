#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pdoc3
PKG_VERSION:=0.10.0
PKG_RELEASE:=1

PYPI_NAME:=pdoc3
PKG_HASH:=5f22e7bcb969006738e1aa4219c75a32f34c2d62d46dc9d2fb2d3e0b0287e4b7

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pdoc3
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Auto-generate API documentation for Python projects.
  URL:=https://pypi.org/project/pdoc3/
  DEPENDS:= \
	+python3-ha-mako \
	+python3-ha-markdown
endef

define Package/python3-ha-pdoc3/description
 PDOC auto-generate API documentation for Python projects..
endef

$(eval $(call Py3Package,python3-ha-pdoc3))
$(eval $(call BuildPackage,python3-ha-pdoc3))
