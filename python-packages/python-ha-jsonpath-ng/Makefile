#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-jsonpath-ng
PKG_VERSION:=1.5.2
PKG_RELEASE:=1
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

PYPI_NAME:=jsonpath-ng
PKG_HASH:=144d91379be14d9019f51973bd647719c877bfc07dc6f3f5068895765950c69d

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-jsonpath-ng
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  URL:=https://github.com/h2non/jsonpath-ng
  TITLE:=python3-jsonpath-ng
  DEPENDS:= \
	+python3-ha-ply \
	+python3-ha-six \
	+python3-ha-decorator
endef

$(eval $(call Py3Package,python3-ha-jsonpath-ng))
$(eval $(call BuildPackage,python3-ha-jsonpath-ng))

