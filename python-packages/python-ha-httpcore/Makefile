#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-httpcore
PKG_VERSION:=0.15.0
PKG_RELEASE:=1

PYPI_NAME:=httpcore
PKG_HASH:=18b68ab86a3ccf3e7dc0f43598eaddcf472b602aba29f9aa6ab85fe2ada3980b

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-httpcore
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=A minimal low-level HTTP client.
  URL:=https://pypi.org/project/httpcore/
  DEPENDS:= \
	+python3-ha-h11 \
	+python3-ha-sniffio \
	+python3-ha-anyio
endef

define Package/python3-ha-httpcore/description
 The HTTP Core package provides a minimal low-level HTTP client, which does one
 thing only. Sending HTTP requests.
endef

$(eval $(call Py3Package,python3-ha-httpcore))
$(eval $(call BuildPackage,python3-ha-httpcore))
