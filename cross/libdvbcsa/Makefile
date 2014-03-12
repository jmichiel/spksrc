PKG_NAME = libdvbcsa
PKG_VERS = 1.1.0
PKG_EXT = tar.gz
PKG_DIST_NAME = $(PKG_NAME)-$(PKG_VERS).$(PKG_EXT)
PKG_DIST_SITE = http://download.videolan.org/pub/videolan/libdvbcsa/$(PKG_VERS)
PKG_DIR = $(PKG_NAME)-$(PKG_VERS)

HOMEPAGE = http://www.videolan.org/developers/libdvbcsa.html
COMMENT  = libdvbcsa is a free implementation of the DVB Common Scrambling Algorithm - DVB/CSA - with encryption and decryption capabilities.
LICENSE  = GPL

GNU_CONFIGURE = 1
CONFIGURE_ARGS = --enable-uint32
INSTALL_TARGET = myInstall

include ../../mk/spksrc.cross-cc.mk


.PHONY: myInstall
myInstall:
	$(RUN) make install DESTDIR=$(INSTALL_DIR)
