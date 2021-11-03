#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-multidict
PKG_VERSION:=4.5.2
PKG_RELEASE:=2

PYPI_NAME:=multidict
PKG_HASH:=024b8129695a952ebd93373e45b5d341dbb87c17ce49637b34000093f243dd4f

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-multidict
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=multidict implementation
  URL:=https://github.com/aio-libs/multidict
  DEPENDS:= \
      +python3-light \
      +python3-ha-attrs
endef

define Package/python3-ha-multidict/description
Multidict is dict-like collection of key-value pairs where key might be occurred more than once in the container.
endef

$(eval $(call Py3Package,python3-ha-multidict))
$(eval $(call BuildPackage,python3-ha-multidict))

