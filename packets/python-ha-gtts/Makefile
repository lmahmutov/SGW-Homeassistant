#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-gtts
PKG_VERSION:=2.2.3
PKG_RELEASE:=1

PYPI_NAME:=gTTS
PKG_HASH:=88cfaa112471867009a0450a696e5bc69cf1671fa0fa683fe17d0650023c863c

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-gtts
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Google Translate text-to-speech API.
  URL:=https://pypi.org/project/gtts/
  DEPENDS:= \
	+python3-ha-click \
	+python3-ha-requests \
	+python3-ha-six
endef

define Package/python3-ha-gtts/description
  gTTS (Google Text-to-Speech), a Python library and CLI tool to interface with
 Google Translate text-to-speech API.
endef

$(eval $(call Py3Package,python3-ha-gtts))
$(eval $(call BuildPackage,python3-ha-gtts))
