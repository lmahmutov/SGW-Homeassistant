#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-coloredlogs
PKG_VERSION:=15.0.1
PKG_RELEASE:=1

PYPI_NAME:=coloredlogs
PKG_HASH:=7c991aa71a4577af2f82600d8f8f3a89f936baeaf9b50a9c197da014e5bf16b0

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-coloredlogs
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Colored terminal output for Python.
  URL:=https://pypi.org/project/coloredlogs/
  DEPENDS:= +python3-light
endef

define Package/python3-ha-coloredlogs/description
 The coloredlogs package enables colored terminal output for Python’s logging module.
 The ColoredFormatter class inherits from logging.Formatter and uses ANSI escape 
 equences to render your logging messages in color.
endef

$(eval $(call Py3Package,python3-ha-coloredlogs))
$(eval $(call BuildPackage,python3-ha-coloredlogs))
