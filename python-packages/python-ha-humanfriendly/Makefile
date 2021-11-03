#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-humanfriendly
PKG_VERSION:=10.0
PKG_RELEASE:=1

PYPI_NAME:=humanfriendly
PKG_HASH:=6b0b831ce8f15f7300721aa49829fc4e83921a9a301cc7f606be6686a2288ddc

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-humanfriendly
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Human friendly output for text.
  URL:=https://pypi.org/project/humanfriendly/
  DEPENDS:= +python3-light
endef

define Package/python3-ha-humanfriendly/description
 Download the file for your platform. If you're not sure which to choose, learn more about.
endef

$(eval $(call Py3Package,python3-ha-humanfriendly))
$(eval $(call BuildPackage,python3-ha-humanfriendly))
