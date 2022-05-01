#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-croniter
PKG_VERSION:=0.3.37
PKG_RELEASE:=1

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE.txt

PYPI_NAME:=croniter
PKG_HASH:=12ced475dfc107bf7c6c1440af031f34be14cd97bbbfaf0f62221a9c11e86404

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-croniter
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=croniter provides iteration for datetime
  URL:=https://pypi.org/project/croniter/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-croniter/description
 croniter provides iteration for datetime object with cron like format.
endef

$(eval $(call Py3Package,python3-ha-croniter))
$(eval $(call BuildPackage,python3-ha-croniter))
