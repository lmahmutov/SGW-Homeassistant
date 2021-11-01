#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-astral
PKG_VERSION:=2.2
PKG_RELEASE:=2

PYPI_NAME:=astral
PKG_HASH:=e41d9967d5c48be421346552f0f4dedad43ff39a83574f5ff2ad32b6627b6fbe

PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-astral
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=(HA CORE) Calculations position of the sun and moon
  URL:=https://github.com/sffjunkie/astral
  DEPENDS+= \
      +python3-light \
      +python3-ha-pytz
endef

define Package/python3-ha-astral/description
Astral is a python module for calculating the times of various aspects of the sun and moon.
endef

$(eval $(call Py3Package,python3-ha-astral))
$(eval $(call BuildPackage,python3-ha-astral))