#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-requests
PKG_VERSION:=2.27.1
PKG_RELEASE:=1

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=LICENSE
PKG_CPE_ID:=cpe:/a:python-requests:requests

PYPI_NAME:=requests
PKG_HASH:=68d7c56fd5a8999887728ef304a6d12edc7be74f1cfa47714fc8b414525c9a61

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
