#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-terminaltables
PKG_VERSION:=3.1.0
PKG_RELEASE:=1

PYPI_NAME:=terminaltables
PKG_HASH:=f3eb0eb92e3833972ac36796293ca0906e998dc3be91fbe1f8615b331b853b81

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-terminaltables
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Generate simple tables in terminals.
  URL:=https://pypi.org/project/terminaltables/
  DEPENDS:= +python3-light
endef

define Package/python3-ha-terminaltables/description
  Easily draw tables in terminal/console applications from a list of lists of strings. Supports multi-line rows.
endef

$(eval $(call Py3Package,python3-ha-terminaltables))
$(eval $(call BuildPackage,python3-ha-terminaltables))