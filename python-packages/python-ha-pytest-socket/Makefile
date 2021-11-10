#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pytest-socket
PKG_VERSION:=0.4.1
PKG_RELEASE:=1

PYPI_NAME:=pytest-socket
PKG_HASH:=b5abcfd14d9c03e7d4e2875bb5e190af28bf5b4162d0a83e3d7aee6d79f1c85d

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pytest-socket
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Pytest Plugin to disable socket calls during tests.
  URL:=https://pypi.org/project/pytest-socket/
  DEPENDS:= +python3-light 
endef

define Package/python3-ha-pytest-socket/description
 A plugin to use with Pytest to disable or restrict
 socket calls during tests to ensure network calls are prevented.
endef

$(eval $(call Py3Package,python3-ha-pytest-socket))
$(eval $(call BuildPackage,python3-ha-pytest-socket))
