#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-markdown
PKG_VERSION:=3.3.3
PKG_RELEASE:=1

PYPI_NAME:=Markdown
PKG_HASH:=5d9f2b5ca24bc4c7a390d22323ca4bad200368612b5aaa7796babf971d2b2f18

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE.md

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-markdown
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Markdown implementation in Python
  URL:=https://python-markdown.github.io/
  DEPENDS:= \
	+python3-light \
	+python3-logging
endef

define Package/python3-ha-markdown/description
  A fast and complete Python implementation of Markdown.
endef

$(eval $(call Py3Package,python3-ha-markdown))
$(eval $(call BuildPackage,python3-ha-markdown))