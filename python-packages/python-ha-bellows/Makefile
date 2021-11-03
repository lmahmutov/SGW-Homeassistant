#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-bellows
PKG_VERSION:=0.28.0
PKG_RELEASE:=1

PYPI_NAME:=bellows
PKG_HASH:=ed84568950e1b79475d528d5f19495a8e5d4b3bb93172856ebe94fc1533e9c4a

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-bellows
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Library implementing EZSP.
  URL:=https://pypi.org/project/bellows/
  DEPENDS:= +python3-light \
	+python3-ha-click \
	+python3-ha-click-log \
	+python3-ha-pure-pcapy3 \
	+python3-ha-pyserial \
	+python3-ha-pyserial-asyncio \
	+python3-ha-voluptuous \
	+python3-ha-zigpy
endef

define Package/python3-ha-bellows/description
  Library implementing EZSP.
endef

$(eval $(call Py3Package,python3-ha-bellows))
$(eval $(call BuildPackage,python3-ha-bellows))
