#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pycares
PKG_VERSION:=4.1.2
PKG_RELEASE:=1

PYPI_NAME:=pycares
PKG_HASH:=03490be0e7b51a0c8073f877bec347eff31003f64f57d9518d419d9369452837

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pycares
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Python interface for c-ares.
  URL:=https://pypi.org/project/pycares/
  DEPENDS:= \
	+python3-light
endef

define Package/python3-ha-pycares/description
 Python interface for c-ares.
endef

$(eval $(call Py3Package,python3-ha-pycares))
$(eval $(call BuildPackage,python3-ha-pycares))
