#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-packaging
PKG_VERSION:=20.4
PKG_RELEASE:=1

PYPI_NAME:=packaging
PKG_HASH:=4357f74f47b9c12db93624a82154e9b120fa8293699949152b22065d556079f8

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0 BSD-2-Clause
PKG_LICENSE_FILES:=LICENSE.APACHE LICENSE.BSD

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-packaging
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Core utilities for Python packages
  URL:=https://github.com/pypa/packaging
  DEPENDS:= \
	+python3-light \
	+python3-ha-pyparsing \
	+python3-ha-six \
	+python3-logging \
	+python3-distutils
endef

define Package/python3-ha-packaging/description
  The packaging project includes version handling, specifiers,
  markers, requirements, tags, utilities.
endef

$(eval $(call Py3Package,python3-ha-packaging))
$(eval $(call BuildPackage,python3-ha-packaging))
