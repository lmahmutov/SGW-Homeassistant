#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-colorlog
PKG_VERSION:=6.4.1
PKG_RELEASE:=1

PYPI_NAME:=colorlog
PKG_HASH:=af99440154a01f27c09256760ea3477982bf782721feaa345904e806879df4d8

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-colorlog
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Add colours to the output of Python's logging.
  URL:=https://pypi.org/project/colorlog/
  DEPENDS:= 
endef

define Package/python3-ha-colorlog/description
 Log formatting with colors!.
endef

$(eval $(call Py3Package,python3-ha-colorlog))
$(eval $(call BuildPackage,python3-ha-colorlog))
