#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-dns
PKG_VERSION:=2.1.0
PKG_RELEASE:=1

PYPI_NAME:=dnspython
PYPI_SOURCE_EXT:=zip
PKG_HASH:=e4a87f0b573201a0f3727fa18a516b055fd1107e0e5477cded4a2de497df1dd4

PKG_LICENSE:=ISC
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-dns
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=dnspython
  URL:=http://www.dnspython.org/
  DEPENDS:=+python3
endef

define Package/python3-ha-dns/description
 dnspython is a DNS toolkit for Python. It supports almost all record types. 
 It can be used for queries, zone transfers, and dynamic updates. It supports TSIG authenticated messages and EDNS0.
endef

$(eval $(call Py3Package,python3-ha-dns))
$(eval $(call BuildPackage,python3-ha-dns))
