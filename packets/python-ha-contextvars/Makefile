#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-contextvars
PKG_VERSION:=2.4
PKG_RELEASE:=1

PYPI_NAME:=contextvars
PKG_HASH:=f38c908aaa59c14335eeea12abea5f443646216c4e29380d7bf34d2018e2c39e

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-contextvars
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=PEP 567 Backport.
  URL:=https://pypi.org/project/contextvars/
  DEPENDS:=+python3-ha-immutables
endef

define Package/python3-ha-contextvars/description
  This package implements a backport of Python 3.7 contextvars module (see PEP 567) for Python 3.6..
endef

$(eval $(call Py3Package,python3-ha-contextvars))
$(eval $(call BuildPackage,python3-ha-contextvars))
