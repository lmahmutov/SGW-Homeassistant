#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-httplib2
PKG_VERSION:=0.20.4
PKG_RELEASE:=1

PYPI_NAME:=httplib2
PKG_HASH:=58a98e45b4b1a48273073f905d2961666ecf0fbac4250ea5b47aef259eb5c585

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-httplib2
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Small, fast HTTP client library for Python.
  URL:=https://pypi.org/project/httplib2/
  DEPENDS:=+python3-light \
	+python3-ha-pyparsing
endef

define Package/python3-ha-httplib2/description
  Small, fast HTTP client library for Python. Features persistent connections,
 cache, and Google App Engine support. Originally written by Joe Gregorio,
 now supported by community.
endef

$(eval $(call Py3Package,python3-ha-httplib2))
$(eval $(call BuildPackage,python3-ha-httplib2))
