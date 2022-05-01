#
# Copyright (C) 2020-2021 CZ.NIC, z. s. p. o. (https://www.nic.cz/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pytest
PKG_VERSION:=6.2.5
PKG_RELEASE:=1

PYPI_NAME:=pytest
PKG_HASH:=131b36680866a76e6781d13f101efb86cf674ebb9762eb70d3082b6f29889e89

PKG_MAINTAINER:=Jan Pavlinec <jan.pavlinec@nic.cz>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

HOST_PYTHON3_PACKAGE_BUILD_DEPENDS:=setuptools-scm

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pytest
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Python testing framework
  URL:=https://docs.pytest.org/en/latest/
  DEPENDS:= \
	+python3 \
	+python3-ha-more-itertools \
	+python3-ha-py \
	+python3-ha-attrs \
	+python3-ha-pluggy \
	+python3-ha-packaging \
	+python3-ha-toml \
	+python3-ha-iniconfig
endef

define Package/python3-ha-pytest/description
  The pytest framework makes it easy to write small tests, yet scales to support
  complex functional testing for applications and libraries.
endef

$(eval $(call Py3Package,python3-ha-pytest))
$(eval $(call BuildPackage,python3-ha-pytest))
$(eval $(call BuildPackage,python3-ha-pytest-src))
