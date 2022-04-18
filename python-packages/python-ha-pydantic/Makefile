#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pydantic
PKG_VERSION:=1.9.0
PKG_RELEASE:=1

PYPI_NAME:=pydantic
PKG_HASH:=742645059757a56ecd886faf4ed2441b9c0cd406079c2b4bee51bcc3fbcd510a

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pydantic
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Data validation and settings management using Python type hinting.
  URL:=https://pypi.org/project/pydantic/
  DEPENDS:= \
	+python3-light
endef

define Package/python3-ha-pydantic/description
 Data validation and settings management using Python type hinting.
endef

$(eval $(call Py3Package,python3-ha-pydantic))
$(eval $(call BuildPackage,python3-ha-pydantic))
