#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-tabulate
PKG_VERSION:=0.8.9
PKG_RELEASE:=1

PYPI_NAME:=tabulate
PKG_HASH:=eb1d13f25760052e8931f2ef80aaf6045a6cceb47514db8beab24cded16f13a7

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-tabulate
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Pretty-print tabular data
  URL:=https://pypi.org/project/tabulate/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-tabulate/description
  Pretty-print tabular data in Python, a library and a command-line utility.
endef

$(eval $(call Py3Package,python3-ha-tabulate))
$(eval $(call BuildPackage,python3-ha-tabulate))
