#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-natsort
PKG_VERSION:=8.0.0
PKG_RELEASE:=1

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE.txt

PYPI_NAME:=natsort
PKG_HASH:=a0a4fd71aee20a6d648da61e01180a63f7268e69983d0440bd3ad80ef1ba6981

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-natsort
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Simple yet flexible natural sorting
  URL:=https://pypi.org/project/natsort/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-natsort/description
 Simple yet flexible natural sorting in Python.
endef

$(eval $(call Py3Package,python3-ha-natsort))
$(eval $(call BuildPackage,python3-ha-natsort))
