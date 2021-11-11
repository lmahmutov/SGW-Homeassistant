#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-protobuf
PKG_VERSION:=3.19.1
PKG_RELEASE:=1

PYPI_NAME:=protobuf
PKG_HASH:=62a8e4baa9cb9e064eb62d1002eca820857ab2138440cb4b3ea4243830f94ca7

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=3-Clause BSD License
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-protobuf
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Protocol Buffers
  URL:=https://pypi.org/project/protobuf/
  DEPENDS:=+python3
endef

define Package/python3-ha-protobuf/description
  Protocol Buffers are Google’s data interchange format.
endef

$(eval $(call Py3Package,python3-ha-protobuf))
$(eval $(call BuildPackage,python3-ha-protobuf))

