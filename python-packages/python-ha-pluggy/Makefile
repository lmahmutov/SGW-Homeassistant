#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pluggy
PKG_VERSION:=0.13.1
PKG_RELEASE:=4

PYPI_NAME:=pluggy
PKG_HASH:=15b2acde666561e1298d71b523007ed7364de07029219b604cf808bfa1c765b0

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

HOST_PYTHON3_PACKAGE_BUILD_DEPENDS:=setuptools-scm

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pluggy
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Plugin and hook calling mechanisms for Python
  URL:=https://github.com/pytest-dev/pluggy
  DEPENDS:=+python3-light
endef

define Package/python3-ha-pluggy/description
  A minimalist production ready plugin system for python
endef

$(eval $(call Py3Package,python3-ha-pluggy))
$(eval $(call BuildPackage,python3-ha-pluggy))
