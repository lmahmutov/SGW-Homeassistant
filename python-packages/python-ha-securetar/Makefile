#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-securetar
PKG_VERSION:=2022.02.0
PKG_RELEASE:=1

PYPI_NAME:=securetar
PKG_SOURCE:=$(PYPI_NAME)-$(PKG_VERSION).tar.gz
PKG_SOURCE_URL:=https://codeload.github.com/pvizeli/securetar/tar.gz/$(PKG_VERSION)?
PKG_HASH:=3b5daa6815799c88d79eca3f3d72629830e3cada73c2086cf425f4f1ee365b26

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0 MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-securetar
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Secure Tar.
  URL:=https://github.com/pvizeli/securetar
  DEPENDS:= \
	+python3-setuptools
endef

define Package/python3-ha-securetar/description
    It's a streaming wrapper around python tarfile and allow secure handling files and support encryption.
endef

$(eval $(call Py3Package,python3-ha-securetar))
$(eval $(call BuildPackage,python3-ha-securetar))
