#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-iniconfig
PKG_VERSION:=1.1.1
PKG_RELEASE:=1

PYPI_NAME:=iniconfig
PKG_HASH:=bc3af051d7d14b2ee5ef9969666def0cd1a000e121eaea580d4a313df4b37f32

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

HOST_PYTHON3_PACKAGE_BUILD_DEPENDS:=setuptools-scm

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-iniconfig
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Simple config-ini parser
  URL:=https://github.com/RonnyPfannschmidt/iniconfig
  DEPENDS:= +python3-light
endef

define Package/python3-ha-iniconfig/description
  iniconfig is a small and simple INI-file parser module.
endef

$(eval $(call Py3Package,python3-ha-iniconfig))
$(eval $(call BuildPackage,python3-ha-iniconfig))
