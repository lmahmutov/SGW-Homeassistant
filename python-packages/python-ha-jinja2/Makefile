#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-jinja2
PKG_VERSION:=3.0.3
PKG_RELEASE:=$(AUTORELEASE)

PYPI_NAME:=Jinja2
PKG_HASH:=611bb273cd68f3b993fabdc4064fc858c5b47a973cb5aa7999ec1ba405c87cd7

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE
PKG_CPE_ID:=cpe:/a:pocoo:jinja2

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-jinja2
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=(HA CORE) Jinja2
  URL:=https://palletsprojects.com/p/jinja/
  DEPENDS:= \
	+python3-light \
	+python3-ha-markupsafe
endef

define Package/python3-ha-jinja2/description
Jinja2 is a full featured template engine for Python. It has full
unicode support, an optional integrated sandboxed execution
environment, widely used and BSD licensed.
endef

$(eval $(call Py3Package,python3-ha-jinja2))
$(eval $(call BuildPackage,python3-ha-jinja2))

