#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-dateutil
PKG_VERSION:=2.8.1
PKG_RELEASE:=3
PKG_LICENSE:=BSD-2-Clause

PYPI_NAME:=python-dateutil
PKG_HASH:=73ebfe9dbf22e832286dafa60473e4cd239f8592f699aa5adaf10050e6e1823c
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

HOST_PYTHON3_PACKAGE_BUILD_DEPENDS:=setuptools-scm

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-dateutil
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Extensions to the standard Python datetime module
  URL:=https://dateutil.readthedocs.org/
  DEPENDS:= \
	+python3 \
	+python3-ha-six
endef

define Package/python3-ha-dateutil/description
  Extensions to the standard Python datetime module
endef

$(eval $(call Py3Package,python3-ha-dateutil))
$(eval $(call BuildPackage,python3-ha-dateutil))
