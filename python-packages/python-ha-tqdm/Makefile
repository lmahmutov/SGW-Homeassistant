#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-tqdm
PKG_VERSION:=4.62.3
PKG_RELEASE:=1

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE.txt

PYPI_NAME:=tqdm
PKG_HASH:=d359de7217506c9851b7869f3708d8ee53ed70a1b8edbba4dbcb47442592920d

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-tqdm
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Fast, Extensible Progress Meter
  URL:=https://pypi.org/project/tqdm/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-tqdm/description
 Fast, Extensible Progress Meter.
endef

$(eval $(call Py3Package,python3-ha-tqdm))
$(eval $(call BuildPackage,python3-ha-tqdm))
