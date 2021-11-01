#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-slugify
PKG_VERSION:=4.0.1
PKG_RELEASE:=1

PYPI_NAME:=python-slugify
PKG_HASH:=69a517766e00c1268e5bbfc0d010a0a8508de0b18d30ad5a1ff357f8ae724270

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-slugify
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=(HA CORE) Slugify application that handles Unicode
  URL:=https://github.com/un33k/python-slugify
  DEPENDS:= \
    +python3-light \
    +python3-codecs \
    +python3-setuptools \
    +python3-ha-text-unidecode
endef

define Package/python3-ha-slugify/description
  A Python slugify application that handles unicode.
endef

$(eval $(call Py3Package,python3-ha-slugify))
$(eval $(call BuildPackage,python3-ha-slugify))
