#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-zha-quirks
PKG_VERSION:=0.0.71
PKG_RELEASE:=1

PYPI_NAME:=zha-quirks
PKG_HASH:=4702cdb5a07ad4f92e0f5ac98334a2a463e7f96c44a1fd513c9e552ccfd57e02

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-zha-quirks
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Zigpy quirks for ZHA in Home Assistant.
  URL:=https://pypi.org/project/zha-quirks/
  DEPENDS:= +python3-light
endef

define Package/python3-ha-zha-quirks/description
 ZHA Device Handlers For Home Assistant.
endef

$(eval $(call Py3Package,python3-ha-zha-quirks))
$(eval $(call BuildPackage,python3-ha-zha-quirks))
