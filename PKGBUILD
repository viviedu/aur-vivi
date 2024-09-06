# Maintainer: Jake Barnes <me+aur@jakebarn.es>
pkgname=vivi
pkgver=3.8.3
pkgrel=1
pkgdesc="Client for Vivi, a wireless screen sharing solution"
arch=('x86_64')
url="http://vivi.io"
license=('unknown')
depends=('gtk3' 'libxss' 'nss' 'glib2' 'libpulse' 'libx11')
source=("${pkgname}-${pkgver}.deb::https://downloads.vivi.io/app/${pkgname}-${pkgver}.deb")
md5sums=('bd055d6fc2ce2fcae2cf0b746d57fa91')

package() {
  msg2 "Extracting the data.tar.xz..."
  bsdtar -xf data.tar.xz -C "$pkgdir/"
}
