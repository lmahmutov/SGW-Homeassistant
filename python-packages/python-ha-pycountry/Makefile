#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pycountry
PKG_VERSION:=22.3.5
PKG_RELEASE:=1

PYPI_NAME:=pycountry
PKG_HASH:=b2163a246c585894d808f18783e19137cb70a0c18fb36748dc01fc6f109c1646

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pycountry
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=pycountry provides the ISO databases.
  URL:=https://pypi.org/project/pycountry/
  DEPENDS:= \
	+python3-light
endef

define Package/python3-ha-pycountry/description
 ISO country, subdivision, language, currency and script definitions and their translations.
endef

$(eval $(call Py3Package,python3-ha-pycountry))
$(eval $(call BuildPackage,python3-ha-pycountry))
