# Maintainer: Jake Barnes <me+aur@jakebarn.es>
pkgname=vivi
pkgver=9.9.9
pkgrel=1
pkgdesc="Client for Vivi, a wireless screen sharing solution"
arch=('x86_64')
url="http://vivi.io"
license=('unknown')
depends=('electron' 'glib2' 'libpulse' 'libx11')
source=(
  "${pkgname}-${pkgver}.deb::https://downloads.vivi.io/app/${pkgver}/${pkgname}.deb"
  vivi
)
md5sums=(
  'SKIP'
  'SKIP'
)

package() {
  msg2 "Extracting the data.tar.xz..."
  mkdir -p "$srcdir/data/"
  bsdtar -xf data.tar.xz -C "$srcdir/data/"
  msg2 "Installing files..."
  install -Dm 755 vivi "$pkgdir/usr/bin/vivi"
  install -Dm 644 "$srcdir/data/usr/lib/vivi/resources/app.asar" "$pkgdir/usr/lib/vivi/app.asar"
  install -Dm 644 "$srcdir/data/usr/share/applications/vivi.desktop" "$pkgdir/usr/share/applications/vivi.desktop"
  install -Dm 644 "$srcdir/data/usr/share/icons/hicolor/128x128/apps/vivi.png" "$pkgdir/usr/share/icons/hicolor/128x128/apps/vivi.png"
  install -Dm 644 "$srcdir/data/usr/share/icons/hicolor/scalable/apps/vivi.svg" "$pkgdir/usr/share/icons/hicolor/scalable/apps/vivi.svg"
}
