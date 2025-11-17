pkgname=fuzzy-pacman
pkgver=1.0.0
pkgrel=1
pkgdesc="Fuzzy pacman wrapper using skim (sk). Provides interactive package and system management via subcommands."
arch=('any')
url="https://github.com/brunos3d/fuzzy-pacman"
license=('MIT')
depends=('pacman' 'skim')
source=("fpm" "fpm.1")
sha256sums=('SKIP' 'SKIP')

package() {
  install -Dm755 "$srcdir/fpm" "$pkgdir/usr/bin/fpm"
  install -Dm644 "$srcdir/fpm.1" "$pkgdir/usr/share/man/man1/fpm.1"
}
