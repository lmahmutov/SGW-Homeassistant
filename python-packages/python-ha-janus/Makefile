#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-janus
PKG_VERSION:=0.6.2
PKG_RELEASE:=1

PYPI_NAME:=janus
PKG_HASH:=127edc891f9e13420dd12f230d5113fa3de7f93662b81acfaf845989edf5eebf

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=COPYING

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-janus
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Mixed sync-async queue
  URL:=https://pypi.org/project/janus/
  DEPENDS:= \
	  +python3-light
endef

define Package/python3-ha-janus/description
  Mixed sync-async queue
endef

$(eval $(call Py3Package,python3-ha-janus))
$(eval $(call BuildPackage,python3-ha-janus))
