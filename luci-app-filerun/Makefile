# This is free software, licensed under the Apache License, Version 2.0

include $(TOPDIR)/rules.mk

LUCI_TITLE:=LuCI for PHP and FileRun
LUCI_DEPENDS:=+filerun
LUCI_PKGARCH:=all

PKG_LICENSE:=Apache-2.0

include $(TOPDIR)/feeds/luci/luci.mk

define Package/luci-app-filerun/extra_provides
    echo 'libc.so.6'; \
    echo 'librt.so.1';
endef

# call BuildPackage - OpenWrt buildroot signature
