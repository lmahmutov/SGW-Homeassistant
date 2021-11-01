#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-requests
PKG_VERSION:=2.26.0
PKG_RELEASE:=1a

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=LICENSE
PKG_CPE_ID:=cpe:/a:python-requests:requests

PYPI_NAME:=requests
PKG_HASH:=b8aa58f8cf793ffd8782d3d8cb19e66ef36f7aba4353eec859e74678b01b07a7

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-requests
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=(HA CORE) HTTP library for Python
  URL:=https://2.python-requests.org/
  DEPENDS:= \
	  +python3-light  \
	  +python3-ha-chardet  \
	  +python3-ha-idna  \
	  +python3-ha-urllib3  \
	  +python3-ha-certifi \
	  +python3-ha-charset-normalizer
endef

define Package/python3-ha-requests/description
  Requests is the only Non-GMO HTTP library for Python, safe for human consumption
endef

$(eval $(call Py3Package,python3-ha-requests))
$(eval $(call BuildPackage,python3-ha-requests))
