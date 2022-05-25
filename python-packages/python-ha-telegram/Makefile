#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-telegram
PKG_VERSION:=0.0.1
PKG_RELEASE:=1

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE.txt

PYPI_NAME:=telegram
PKG_HASH:=d405a0af4c868a8dbeae6d03e297e21c7ee6269e11e2ed3810e15544aba02591

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-telegram
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Telegram APIs
  URL:=https://pypi.org/project/telegram/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-telegram/description
 Telegram APIs.
endef

$(eval $(call Py3Package,python3-ha-telegram))
$(eval $(call BuildPackage,python3-ha-telegram))
