#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-markupsafe
PKG_VERSION:=2.0.1
PKG_RELEASE:=$(AUTORELEASE)

PYPI_NAME:=MarkupSafe
PKG_HASH:=594c67807fb16238b30c44bdf74f36c02cdf22d1c8cda91ef8a0ed8dabf5620a

PKG_MAINTAINER:=Daniel Golle <daniel@makrotopia.org>
PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE.rst

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-markupsafe
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=MarkupSafe
  URL:=https://palletsprojects.com/p/markupsafe/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-markupsafe/description
  MarkupSafe implements a text object that escapes characters so it is safe to use in HTML and XML.
endef

$(eval $(call Py3Package,python3-ha-markupsafe))
$(eval $(call BuildPackage,python3-ha-markupsafe))
