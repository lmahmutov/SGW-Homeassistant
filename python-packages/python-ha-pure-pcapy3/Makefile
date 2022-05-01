#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pure-pcapy3
PKG_VERSION:=1.0.1
PKG_RELEASE:=1

PYPI_NAME:=pure-pcapy3
PKG_HASH:=b99e45f16d4ad410eb5ebbc7d5d39e353d7eda7e86f0ad52e4dc5c45a7b3ea92

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pure-pcapy3
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Pure Python reimplementation of pcapy.
  URL:=https://pypi.org/project/pure-pcapy3/
  DEPENDS:= +python3-light
endef

define Package/python3-ha-pure-pcapy3/description
  Pure Python reimplementation of pcapy. This package is API compatible and a drop-in replacement.
endef

$(eval $(call Py3Package,python3-ha-pure-pcapy3))
$(eval $(call BuildPackage,python3-ha-pure-pcapy3))
