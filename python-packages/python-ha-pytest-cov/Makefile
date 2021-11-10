#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pytest-cov
PKG_VERSION:=2.12.1
PKG_RELEASE:=1

PYPI_NAME:=pytest-cov
PKG_HASH:=261ceeb8c227b726249b376b8526b600f38667ee314f910353fa318caa01f4d7

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pytest-cov
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Pytest plugin for measuring coverage.
  URL:=https://pypi.org/project/pytest-cov/
  DEPENDS:= +python3-light 
endef

define Package/python3-ha-pytest-cov/description
 This plugin produces coverage reports. 
 Compared to just using coverage run this plugin does some extras.
endef

$(eval $(call Py3Package,python3-ha-pytest-cov))
$(eval $(call BuildPackage,python3-ha-pytest-cov))
