# Maintainer: Emily Johnson <m0k4s4rt@gmail.com>
pkgname=beer
pkgver=1.0.4
pkgrel=1
pkgdesc="Prints 'No, fuck you.' unless run with sudo, then outputs a mug logo"
arch=('any')
url="https://aur.archlinux.org/packages/beer"
license=('GPL-2.0-only')
depends=('bash')
source=('beer' 'mug.txt' 'LICENSE')
sha256sums=('SKIP' 'SKIP' 'SKIP')

package() {
  install -Dm755 "$srcdir/beer" "$pkgdir/usr/bin/beer"
  install -d "$pkgdir/usr/bin"
  ln -s /usr/bin/beer "$pkgdir/usr/bin/Beer"
  install -Dm644 "$srcdir/mug.txt" "$pkgdir/usr/share/beer/mug.txt"
  install -Dm644 "$srcdir/LICENSE" "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
