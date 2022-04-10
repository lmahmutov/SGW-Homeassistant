#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-sqlalchemy
PKG_VERSION:=1.4.32
PKG_RELEASE:=1

PYPI_NAME:=SQLAlchemy
PKG_HASH:=6fdd2dc5931daab778c2b65b03df6ae68376e028a3098eb624d0909d999885bc

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE
PKG_CPE_ID:=cpe:/a:sqlalchemy:sqlalchemy

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-sqlalchemy
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Database Abstraction Library
  URL:=https://www.sqlalchemy.org
  DEPENDS:= \
	+python3-light \
	+python3-urllib \
	+python3-decimal \
	+python3-logging
endef

define Package/python3-ha-sqlalchemy/description
  SQLAlchemy is the Python SQL toolkit and Object Relational Mapper
  that gives application developers the full power and flexibility of SQL.
  SQLAlchemy provides a full suite of well known enterprise-level persistence patterns,
  designed for efficient and high-performing database access,
  adapted into a simple and Pythonic domain language.
endef

$(eval $(call Py3Package,python3-ha-sqlalchemy))
$(eval $(call BuildPackage,python3-ha-sqlalchemy))
