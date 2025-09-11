# Maintainer: Emily Johnson <m0k4s4rt@gmail.com>
pkgname=beer
pkgver=2.0.1
pkgrel=1
pkgdesc="Prints a rude message unless run as root; as root, outputs ASCII art of a mug"
arch=('any')
url="https://github.com/DawnStar907/Beer"
license=('GPL-2.0-only')
depends=('bash')
optdepends=('sudo: convenient way to run as root')
source=('beer' 'LICENSE')
b2sums=('6810cfe97e4437c41d10482fe4f77468b8d1503708c579de8c44cde965a90844c9c6c8e3c57cc3fae204551a20f4e0ff300c0354a50dc65f20349467f428ceef'
        '1e1e108a77d8676eb68467cdfbf95684f0bad991bfcc24e7bd3d1eec58d746f14d20798c3bcf64e9bdd1ff4a9c5ec02ccb4c06331bcf251a9d1d0f28b6875296')

package() {
  install -Dm755 "$srcdir/beer" "$pkgdir/usr/bin/beer"
  ln -s "beer" "$pkgdir/usr/bin/Beer"
  install -Dm644 "$srcdir/LICENSE" "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}

check() {
  if command -v shellcheck >/dev/null 2>&1; then
    # Don’t fail the build on shellcheck findings; just report them.
    shellcheck -s bash "$srcdir/beer" || {
      echo "shellcheck found issues (non-fatal). Review the output above." >&2
      true
    }
  fi
}
