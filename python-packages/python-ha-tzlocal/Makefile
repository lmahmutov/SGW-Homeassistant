#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-tzlocal
PKG_VERSION:=4.1
PKG_RELEASE:=1

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE.txt

PYPI_NAME:=tzlocal
PKG_HASH:=0f28015ac68a5c067210400a9197fc5d36ba9bc3f8eaf1da3cbd59acdfed9e09

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-tzlocal
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=tzinfo object for the local timezone
  URL:=https://pypi.org/project/tzlocal/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-tzlocal/description
 tzinfo object for the local timezone.
endef

$(eval $(call Py3Package,python3-ha-tzlocal))
$(eval $(call BuildPackage,python3-ha-tzlocal))
