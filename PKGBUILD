# Maintainer: pgp <admin@pgpkey.net>
pkgname=pkgsentinel
pkgver=1.0.0
pkgrel=1
pkgdesc="Suspicious File Alert System – warns if pacman alters sensitive files"
arch=('any')
url="https://github.com/pgpz/pkgsentinel"
license=('MIT')
depends=('bash' 'coreutils')
source=("pkgsentinel" "pkgsentinel.hook")
sha256sums=('SKIP' 'SKIP')

package() {
  install -Dm755 "$srcdir/pkgsentinel" "$pkgdir/usr/local/bin/pkgsentinel"
  install -Dm644 "$srcdir/pkgsentinel.hook" "$pkgdir/etc/pacman.d/hooks/pkgsentinel.hook"
}
