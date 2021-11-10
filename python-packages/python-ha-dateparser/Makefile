#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-dateparser
PKG_VERSION:=1.0.0
PKG_RELEASE:=1

PYPI_NAME:=dateparser
PKG_HASH:=159cc4e01a593706a15cd4e269a0b3345edf3aef8bf9278a57dac8adf5bf1e4a

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-dateparser
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Date parsing library.
  URL:=https://pypi.org/project/dateparser/
  DEPENDS:= +python3-light 
endef

define Package/python3-ha-dateparser/description
  Date parsing library designed to parse dates from HTML pages.
endef

$(eval $(call Py3Package,python3-ha-dateparser))
$(eval $(call BuildPackage,python3-ha-dateparser))
