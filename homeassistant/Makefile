#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=homeassistant
PKG_VERSION:=2021.11.2
PKG_RELEASE:=1

PYPI_NAME:=homeassistant
PKG_HASH:=e162d76f76221ee0a0f0f672fb969be03c6f941677b47839e39faee0ea0f93ce

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=LICENSE.md
PKG_CPE_ID:=cpe:/a:home-assistant:home-assistant

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/homeassistant
  CATEGORY:=Homeassistant
  TITLE:=Open source home automation
  URL:=https://github.com/home-assistant/core
  DEPENDS:= \
	+python3-dev \
	+python3-pip
# core
  DEPENDS+= \
	+python3-ha-aiohttp \
	+python3-ha-astral \
	+python3-ha-async-timeout \
	+python3-ha-attrs \
	+python3-ha-awesomeversion \
	+python3-ha-bcrypt \
	+python3-ha-certifi \
	+python3-ha-ciso8601 \
	+python3-ha-cryptography \
	+python3-ha-httpx \
	+python3-ha-jinja2 \
	+python3-ha-pyjwt \
	+python3-ha-requests \
	+python3-ha-ruamel-yaml \
	+python3-ha-slugify \
	+python3-ha-voluptuous \
	+python3-ha-voluptuous-serialize \
	+python3-ha-yaml \
	+python3-ha-yarl \
	+python3-ha-pyturbojpeg
# base
  DEPENDS+= \
	+python3-ha-aiodiscover \
	+python3-ha-aiohttp-cors \
	+python3-ha-async-upnp-client \
	+python3-ha-defusedxml \
	+python3-ha-emoji \
	+python3-hass-nabucasa \
	+python3-home-assistant-frontend \
	+python3-ha-ifaddr \
	+python3-ha-pillow \
	+python3-ha-pynacl \
	+python3-ha-pyserial \
	+python3-ha-pyudev \
	+python3-ha-sqlalchemy \
	+python3-ha-zeroconf \
	+python3-ha-scapy
# ext
  DEPENDS+= \
	+python3-ha-cryptodome \
	+python3-ha-gtts \
	+python3-ha-h11 \
	+python3-ha-httplib2 \
	+python3-ha-mutagen \
	+python3-ha-paho-mqtt \
	+python3-ha-pymetno \
	+python3-ha-pyotp \
	+python3-ha-pyqrcode \
	+python3-ha-urllib3 \
	+python3-ha-websocket-client \
	+python3-ha-xmltodict
endef

define Package/homeassistant/description
  Open source home automation that puts local control and privacy first. Powered by a worldwide community of tinkerers and DIY enthusiasts.
endef

define Py3Package/homeassistant/install
	$(INSTALL_DIR) $(1)/usr/bin 
	$(INSTALL_BIN) $(PKG_INSTALL_DIR)/usr/bin/hass $(1)/usr/bin

	$(INSTALL_DIR) $(1)/etc/init.d
	$(INSTALL_BIN) ./files/S99hass $(1)/etc/init.d

	$(INSTALL_DIR) $(1)/etc/homeassistant
	$(INSTALL_BIN) ./files/installed $(1)/etc/homeassistant

endef

define Package/homeassistant/postrm
#!/bin/sh

rm -rf $(1)$(PYTHON3_PKG_DIR)/$(PKG_NAME)-$(PKG_VERSION)-py$(PYTHON3_VERSION).egg-info
endef

$(eval $(call Py3Package,homeassistant))
$(eval $(call BuildPackage,homeassistant))