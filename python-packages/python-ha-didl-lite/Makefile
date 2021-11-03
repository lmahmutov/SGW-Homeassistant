#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-didl-lite
PKG_VERSION:=1.3.1
PKG_RELEASE:=1

PYPI_NAME:=python-didl-lite
PKG_HASH:=094d4910baa5b014d0f1479ee6716b9c8891612ef8548dfc91f8dbe3b41f997d

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-didl-lite
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:= Tools to read and write DIDL-Lite-xml.
  URL:=https://pypi.org/project/didl-lite/
  DEPENDS:=+python3-ha-defusedxml
endef

define Package/python3-ha-didl-lite/description
 DIDL-Lite tools for Python to read and write DIDL-Lite-xml.
endef

$(eval $(call Py3Package,python3-ha-didl-lite))
$(eval $(call BuildPackage,python3-ha-didl-lite))
