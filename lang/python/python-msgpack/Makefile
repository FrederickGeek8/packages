#
# Copyright (C) 2017-2020 CZ.NIC, z. s. p. o. (https://www.nic.cz/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-msgpack
PKG_VERSION:=1.0.0
PKG_RELEASE:=1

PYPI_NAME:=msgpack
PKG_HASH:=9534d5cc480d4aff720233411a1f765be90885750b07df772380b34c10ecb5c0

PKG_MAINTAINER:=Jan Pavlinec <jan.pavlinec@nic.cz>
PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=COPYING

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-msgpack
  SUBMENU:=Python
  SECTION:=lang
  CATEGORY:=Languages
  TITLE:=MessagePack (de)serializer
  URL:=https://msgpack.org/
  DEPENDS:=+python3-light +libstdcpp
endef

define Package/python3-msgpack/description
  MessagePack is an efficient binary serialization format.
  It lets you exchange data among multiple languages like JSON.
endef

$(eval $(call Py3Package,python3-msgpack))
$(eval $(call BuildPackage,python3-msgpack))
$(eval $(call BuildPackage,python3-msgpack-src))
