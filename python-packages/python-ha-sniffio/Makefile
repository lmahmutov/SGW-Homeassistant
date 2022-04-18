#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-sniffio
PKG_VERSION:=1.2.0
PKG_RELEASE:=1

PYPI_NAME:=sniffio
PKG_HASH:=c4666eecec1d3f50960c6bdf61ab7bc350648da6c126e3cf6898d8cd4ddcd3de

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0 MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-sniffio
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Sniff out which async library.
  URL:=https://pypi.org/project/sniffio/
  DEPENDS:= \
	+python3-ha-contextvars \
	+python3-ha-requires
endef

define Package/python3-ha-sniffio/description
  Sniff out which async library your code is running under.
endef

$(eval $(call Py3Package,python3-ha-sniffio))
$(eval $(call BuildPackage,python3-ha-sniffio))
