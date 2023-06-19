# Maintainer: Rudra Saraswat <rs2009@ubuntu.com>

# This is a barebones PKGBUILD that simply install the AppImages to /usr/bin (proper one pending).

pkgname=zsync2
pkgver=2.0.0.alpha.1
pkgrel=1
pkgdesc='A rewrite of zsync-curl, using modern C++'
arch=(x86_64)
url='https://github.com/AppImageCommunity/zsync2'
depends=('curl')
source=('https://github.com/AppImageCommunity/zsync2/releases/download/2.0.0-alpha-1-20230304/zsync2-63-1608115-x86_64.AppImage'
        'https://github.com/AppImageCommunity/zsync2/releases/download/2.0.0-alpha-1-20230304/zsyncmake2-63-1608115-x86_64.AppImage')
sha512sums=('850c69f5e40f8211a91c0b89fc03bba0a1e5c4d69d5bd31b912546bbab502e71f11541186a6ce5e117142ca774146949818eb3d781c7735cc452d5b3c6dc2a5d'
            '2c6833fbfa275cecd9d2dcfe901067908936df9857b32c5a4f05b33de18a2e074c13e014f3c09bd43dfd6e881d361beccb1c550b2a269f0cb83865f098437477')

OPTIONS=(!strip !docs libtool emptydirs)

package() {
	install -Dm755 zsync2-63-1608115-x86_64.AppImage "${pkgdir}/usr/bin/zsync2"
	install -Dm755 zsyncmake2-63-1608115-x86_64.AppImage "${pkgdir}/usr/bin/zsyncmake2"
}
