# Maintainer: Jake Barnes <me+aur@jakebarn.es>
pkgname=vivi
pkgver=3.9.2
pkgrel=1
pkgdesc="Client for Vivi, a wireless screen sharing solution"
arch=('x86_64')
url="http://vivi.io"
license=('unknown')
depends=('gtk3' 'libxss' 'nss' 'glib2' 'libpulse' 'libx11')
source=("${pkgname}-${pkgver}.deb::https://downloads.vivi.io/app/${pkgname}-${pkgver}.deb")
md5sums=('77f4a226320172104de98317a6d80419')

package() {
  msg2 "Extracting the data.tar.xz..."
  bsdtar -xf data.tar.xz -C "$pkgdir/"
}
