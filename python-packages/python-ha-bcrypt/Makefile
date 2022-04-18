#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=bcrypt
PKG_VERSION:=3.1.7
PKG_RELEASE:=4

PYPI_NAME:=$(PKG_NAME)
PKG_HASH:=0b0069c752ec14172c5f78208f1863d7ad6755a6fae6fe76ec2c80d13be41e42

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=LICENSE

PKG_BUILD_DEPENDS:=libffi/host
HOST_PYTHON3_PACKAGE_BUILD_DEPENDS:=cffi  # cffi>=1.1

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-bcrypt
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=(HA CORE) Modern password hashing
  URL:=https://github.com/pyca/bcrypt/
  DEPENDS:= \
	+python3 \
	+python3-ha-cffi \
	+python3-ha-six
endef

define Package/python3-ha-bcrypt/description
  Good password hashing for your software and your servers.
endef

$(eval $(call Py3Package,python3-ha-bcrypt))
$(eval $(call BuildPackage,python3-ha-bcrypt))

