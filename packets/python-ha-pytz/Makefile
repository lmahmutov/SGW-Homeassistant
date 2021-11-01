#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pytz
PKG_VERSION:=2021.1
PKG_RELEASE:=1

PYPI_NAME:=pytz
PKG_HASH:=83a4a90894bf38e243cf052c8b58f381bfe9a7a483f6a9cab140bc7f702ac4da

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE.txt

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pytz
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=World timezone definitions, modern and historical
  URL:=https://pythonhosted.org/pytz/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-pytz/description
  World timezone definitions, modern and historical
endef

$(eval $(call Py3Package,python3-ha-pytz))
$(eval $(call BuildPackage,python3-ha-pytz))

