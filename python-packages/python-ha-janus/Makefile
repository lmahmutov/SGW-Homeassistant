#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-janus
PKG_VERSION:=1.0.0
PKG_RELEASE:=1

PYPI_NAME:=janus
PKG_HASH:=df976f2cdcfb034b147a2d51edfc34ff6bfb12d4e2643d3ad0e10de058cb1612

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
