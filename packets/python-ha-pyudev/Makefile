#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pyudev
PKG_VERSION:=0.22.0
PKG_RELEASE:=1

PYPI_NAME:=pyudev
PKG_HASH:=69bb1beb7ac52855b6d1b9fe909eefb0017f38d917cba9939602c6880035b276

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=LGPL-2.1-or-later
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pyudev
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=A libudev binding.
  URL:=https://pypi.org/project/pyudev/
  DEPENDS:= \
	+python3-ha-six \
	+libudev-zero
endef

define Package/python3-ha-pyudev/description
  Python bindings to libudev (with support for PyQt4, PySide, pygobject and wx).
endef

$(eval $(call Py3Package,python3-ha-pyudev))
$(eval $(call BuildPackage,python3-ha-pyudev))
