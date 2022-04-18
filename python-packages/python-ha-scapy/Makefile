#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-scapy
PKG_VERSION:=2.4.5
PKG_RELEASE:=1

PYPI_NAME:=scapy
PKG_HASH:=bc707e3604784496b6665a9e5b2a69c36cc9fb032af4864b29051531b24c8593

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=GPL-2.0-only
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-scapy
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Interactive packet manipulation tool and network scanner
  URL:=https://scapy.net/
  DEPENDS:=+python3
endef

define Package/python3-ha-scapy/description
  Scapy is a powerful interactive packet manipulation program built on top
  of the Python interpreter. It can be used to forge or decode packets of
  a wide number of protocols, send them over the wire, capture them, match
  requests and replies, and much more.
endef

$(eval $(call Py3Package,python3-ha-scapy))
$(eval $(call BuildPackage,python3-ha-scapy))

