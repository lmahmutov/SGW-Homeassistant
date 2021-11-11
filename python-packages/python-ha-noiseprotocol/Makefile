#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-noiseprotocol
PKG_VERSION:=0.3.1
PKG_RELEASE:=1

PYPI_NAME:=noiseprotocol
PKG_HASH:=b092a871b60f6a8f07f17950dc9f7098c8fe7d715b049bd4c24ee3752b90d645

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=3-Clause BSD License
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-noiseprotocol
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Noise Protocol Framework
  URL:=https://pypi.org/project/noiseprotocol/
  DEPENDS:=+python3
endef

define Package/python3-ha-noiseprotocol/description
 Python 3 implementation of Noise Protocol Framework.
endef

$(eval $(call Py3Package,python3-ha-noiseprotocol))
$(eval $(call BuildPackage,python3-ha-noiseprotocol))

