#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-click-log
PKG_VERSION:=0.3.2
PKG_RELEASE:=2
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

PYPI_NAME:=click-log
PKG_HASH:=16fd1ca3fc6b16c98cea63acf1ab474ea8e676849dc669d86afafb0ed7003124
PKG_LICENSE:=MIT

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-click-log
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  URL:=http://github.com/mitsuhiko/click
  TITLE:=python3-click-log
  DEPENDS:=+python3-ha-click
endef

define Package/python3-ha-click-log/description
  Simple and beautiful logging for click applications
endef

$(eval $(call Py3Package,python3-ha-click-log))
$(eval $(call BuildPackage,python3-ha-click-log))
