#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-aiodiscover
PKG_VERSION:=1.4.8
PKG_RELEASE:=1

PYPI_NAME:=aiodiscover
PKG_HASH:=7babac7741b42bf614f7e1e4a144d36846226d18444d35abf824262298539db1

PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-aiodiscover
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Discover hosts by arp and ptr lookup
  URL:=https://pypi.org/project/aiodiscover/
  DEPENDS:= \
	+python3-ha-dns \
	+python3-ha-ifaddr \
	+python3-ha-pyroute2
endef

define Package/python3-ha-aiodiscover/description
  Discover hosts on the network via ARP and PTR lookup.
endef

$(eval $(call Py3Package,python3-ha-aiodiscover))
$(eval $(call BuildPackage,python3-ha-aiodiscover))
