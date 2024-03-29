#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=homeassistant
PKG_VERSION:=2022.6.2
PKG_RELEASE:=1

PYPI_NAME:=homeassistant
PKG_HASH:=c13bedd18e38266519be110bb45e51f5038157bca9b51dedc712cde32e2aaead

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
  USERID:=homeassistant:homeassistant
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
	+python3-ha-pyturbojpeg \
	+python3-ha-securetar
# base
  DEPENDS+= \
	+python3-ha-aiodiscover \
	+python3-ha-aiohttp-cors \
	+python3-ha-async-upnp-client \
	+python3-ha-defusedxml \
	+python3-ha-emoji \
	+hass-nabucasa \
	+python3-home-assistant-frontend \
	+python3-ha-ifaddr \
	+python3-ha-pillow \
	+python3-ha-pynacl \
	+python3-ha-pyserial \
	+python3-ha-pyudev \
	+python3-ha-sqlalchemy \
	+python3-ha-zeroconf \
	+python3-ha-scapy \
	+python3-ha-lru-dict \
	+python3-ha-fnvhash
# ext
  DEPENDS+= \
	+libpcap \
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
	+python3-ha-xmltodict \
	+python3-ha-radios \
	+python3-ha-pycares \
	+python3-ha-hatasmota \
	+python3-ha-telegram
endef

define Package/homeassistant/description
  Open source home automation that puts local control and privacy first. Powered by a worldwide community of tinkerers and DIY enthusiasts.
endef

define Build/Prepare
	$(call Build/Prepare/Default)
	# serve static with gzipped files
	sed -i 's/filepath = self._directory.joinpath(filename).resolve()/try:\n                filepath = self._directory.joinpath(Path(rel_url + ".gz")).resolve()\n                if not filepath.exists():\n                    raise FileNotFoundError()\n            except Exception as e:\n                filepath = self._directory.joinpath(filename).resolve()/' $(PKG_BUILD_DIR)/homeassistant/components/http/static.py
	# Remove cloud
	sed -i 's/"cloud",//' $(PKG_BUILD_DIR)/homeassistant/components/default_config/manifest.json
	# Remove unwanted integrations
	sed -i 's/    "/    # "/' $(PKG_BUILD_DIR)/homeassistant/generated/config_flows.py
	sed -i 's/    # "integration":/    "integration":/' $(PKG_BUILD_DIR)/homeassistant/generated/config_flows.py
	sed -i 's/    # "mqtt"/    "mqtt"/' $(PKG_BUILD_DIR)/homeassistant/generated/config_flows.py
	sed -i 's/    # "zha"/    "zha"/' $(PKG_BUILD_DIR)/homeassistant/generated/config_flows.py
	sed -i 's/    # "esphome"/    "esphome"/' $(PKG_BUILD_DIR)/homeassistant/generated/config_flows.py
	sed -i 's/    # "wled"/    "wled"/' $(PKG_BUILD_DIR)/homeassistant/generated/config_flows.py
	sed -i 's/    # "homekit"/    "homekit"/' $(PKG_BUILD_DIR)/homeassistant/generated/config_flows.py
	sed -i 's/    # "homekit_controller"/    "homekit_controller"/' $(PKG_BUILD_DIR)/homeassistant/generated/config_flows.py
	sed -i 's/    # "tasmota"/    "tasmota"/' $(PKG_BUILD_DIR)/homeassistant/generated/config_flows.py
	sed -i 's/    # "xiaomi_miio"/    "xiaomi_miio"/' $(PKG_BUILD_DIR)/homeassistant/generated/config_flows.py
	sed -i 's/    # "yeelight"/    "yeelight"/' $(PKG_BUILD_DIR)/homeassistant/generated/config_flows.py
	sed -i 's/    # "yeelightsunflower"/    "yeelightsunflower"/' $(PKG_BUILD_DIR)/homeassistant/generated/config_flows.py
	sed -i 's/    # "helper":/    "helper":/' $(PKG_BUILD_DIR)/homeassistant/generated/config_flows.py
	sed -i 's/    # "derivative",/    "derivative",/' $(PKG_BUILD_DIR)/homeassistant/generated/config_flows.py
	sed -i 's/    # "group",/    "group",/' $(PKG_BUILD_DIR)/homeassistant/generated/config_flows.py
	sed -i 's/    # "integration",/    "integration",/' $(PKG_BUILD_DIR)/homeassistant/generated/config_flows.py
	sed -i 's/    # "min_max",/    "min_max",/' $(PKG_BUILD_DIR)/homeassistant/generated/config_flows.py
	sed -i 's/    # "switch_as_x",/    "switch_as_x",/' $(PKG_BUILD_DIR)/homeassistant/generated/config_flows.py
	sed -i 's/    # "threshold",/    "threshold",/' $(PKG_BUILD_DIR)/homeassistant/generated/config_flows.py
	sed -i 's/    # "tod",/    "tod",/' $(PKG_BUILD_DIR)/homeassistant/generated/config_flows.py
	sed -i 's/    # "utility_meter"/    "utility_meter"/' $(PKG_BUILD_DIR)/homeassistant/generated/config_flows.py

	# disabling all zeroconf services
	sed -i 's/^    "_/    "_disabled_/' $(PKG_BUILD_DIR)/homeassistant/generated/zeroconf.py
	# re-enable required ones
	sed -i 's/_disabled_esphomelib./_esphomelib./' $(PKG_BUILD_DIR)/homeassistant/generated/zeroconf.py
	sed -i 's/_disabled_homekit._tcp.local./_homekit._tcp.local./' $(PKG_BUILD_DIR)/homeassistant/generated/zeroconf.py
	sed -i 's/_disabled_ipps./_ipps./' $(PKG_BUILD_DIR)/homeassistant/generated/zeroconf.py
	sed -i 's/_disabled_ipp./_ipp./' $(PKG_BUILD_DIR)/homeassistant/generated/zeroconf.py
	sed -i 's/_disabled_printer./_printer./' $(PKG_BUILD_DIR)/homeassistant/generated/zeroconf.py
	sed -i 's/_disabled_miio./_miio./' $(PKG_BUILD_DIR)/homeassistant/generated/zeroconf.py
	#update version
	sed -i 's/version=.*/version="$(PKG_VERSION)",/' $(PKG_BUILD_DIR)/setup.py
	#downgrade python cryptograpy untill RUST is available
	sed -i 's/cryptography==.*/cryptography==3.4.8/' $(PKG_BUILD_DIR)/homeassistant.egg-info/requires.txt
	sed -i 's/cryptography==.*/cryptography==3.4.8/' $(PKG_BUILD_DIR)/homeassistant/package_constraints.txt
	sed -i 's/cryptography==.*/cryptography==3.4.8/' $(PKG_BUILD_DIR)/setup.cfg
endef

define Py3Package/homeassistant/install
	$(INSTALL_DIR) $(1)/usr/bin 
	$(INSTALL_BIN) $(PKG_INSTALL_DIR)/usr/bin/hass $(1)/usr/bin

	$(INSTALL_DIR) $(1)/etc/init.d
	$(INSTALL_BIN) ./files/homeassistant $(1)/etc/init.d

	$(INSTALL_DIR) $(1)/etc/homeassistant
	$(INSTALL_BIN) ./files/installed $(1)/etc/homeassistant
endef

define Package/homeassistant/postrm
#!/bin/sh

rm -rf $(1)$(PYTHON3_PKG_DIR)/$(PKG_NAME)-$(PKG_VERSION)-py$(PYTHON3_VERSION).egg-info
endef

$(eval $(call Py3Package,homeassistant))
$(eval $(call BuildPackage,homeassistant))