#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-charset-normalizer
PKG_VERSION:=2.0.4
PKG_RELEASE:=1

PYPI_NAME:=charset-normalizer
PKG_HASH:=f23667ebe1084be45f6ae0538e4a5a865206544097e4e8bbcacf42cd02a348f3

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-charset-normalizer
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=The Real First Universal Charset Detector.
  URL:=https://pypi.org/project/charset-normalizer/
  DEPENDS:= +python3-light
endef

define Package/python3-ha-charset-normalizer/description
  The Real First Universal Charset Detector. Open, modern and actively maintained alternative to Chardet.
endef

$(eval $(call Py3Package,python3-ha-charset-normalizer))
$(eval $(call BuildPackage,python3-ha-charset-normalizer))
