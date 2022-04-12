#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-lru-dict
PKG_VERSION:=1.1.7
PKG_RELEASE:=1

PYPI_NAME:=lru-dict
PKG_HASH:=45b81f67d75341d4433abade799a47e9c42a9e22a118531dcb5e549864032d7c

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0 MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-lru-dict
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=An Dict like LRU container.
  URL:=https://pypi.org/project/lru-dict/
  DEPENDS:= \
	+python3-setuptools
endef

define Package/python3-ha-lru-dict/description
  A fixed size dict like container which evicts Least Recently Used (LRU) items
  once size limit is exceeded. There are many python implementations available
  which does similar things
endef

$(eval $(call Py3Package,python3-ha-lru-dict))
$(eval $(call BuildPackage,python3-ha-lru-dict))
