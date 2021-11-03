#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-voluptuous
PKG_VERSION:=0.12.2
PKG_RELEASE:=1

PYPI_NAME:=voluptuous
PKG_HASH:=4db1ac5079db9249820d49c891cb4660a6f8cae350491210abce741fabf56513

PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=COPYING
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-voluptuous
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=(HA CORE) Data validation library
  URL:=https://github.com/alecthomas/voluptuous
  DEPENDS:= \
      +python3-light
endef

define Package/python3-ha-voluptuous/description
It is primarily intended for validating data coming into Python as JSON, YAML, etc.
endef

$(eval $(call Py3Package,python3-ha-voluptuous))
$(eval $(call BuildPackage,python3-ha-voluptuous))
