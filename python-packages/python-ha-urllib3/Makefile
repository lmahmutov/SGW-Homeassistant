#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-urllib3
PKG_VERSION:=1.26.9
PKG_RELEASE:=1

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE.txt
PKG_CPE_ID:=cpe:/a:urllib3_project:urllib3

PYPI_NAME:=urllib3
PKG_HASH:=aabaf16477806a5e1dd19aa41f8c2b7950dd3c746362d7e3223dbe6de6ac448e

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-urllib3
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Sanity-friendly HTTP client
  URL:=https://urllib3.readthedocs.io/
  DEPENDS:=+python3
endef

define Package/python3-ha-urllib3/description
  HTTP library with thread-safe connection pooling, file post, and more.
endef

$(eval $(call Py3Package,python3-ha-urllib3))
$(eval $(call BuildPackage,python3-ha-urllib3))
