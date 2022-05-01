#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-aiogithubapi
PKG_VERSION:=21.8.1
PKG_RELEASE:=1

PYPI_NAME:=aiogithubapi
PKG_HASH:=92600ff4bbf8e4bbdebbca5bb3f0208bbe7d47a669218c264289ef864c5a3ac6

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-aiogithubapi
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Asynchronous Python client for the GitHub API.
  URL:=https://pypi.org/project/aiogithubapi/
  DEPENDS:= \
	+python3-ha-black \
	+python3-ha-pdoc3 \
	+python3-ha-aiohttp \
	+python3-ha-async-timeout \
	+python3-ha-aresponses \
	+python3-ha-pytest \
	+python3-ha-pytest-cov \
	+python3-ha-pytest-asyncio \
	+python3-ha-backoff
endef

define Package/python3-ha-aiogithubapi/description
  Asynchronous Python client for the GitHub API
 This is not a full client for the API (Have you seen it, it's huge),
 and will probably never be. Things are added when needed or requested.
endef

$(eval $(call Py3Package,python3-ha-aiogithubapi))
$(eval $(call BuildPackage,python3-ha-aiogithubapi))
