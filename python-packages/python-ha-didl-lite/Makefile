#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-didl-lite
PKG_VERSION:=1.3.2
PKG_RELEASE:=1

PYPI_NAME:=python-didl-lite
PKG_HASH:=88c0641d3140f7b05f1efd93f7c481fc62aa50d1e05e17f0e0a15bee025c4af1

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
