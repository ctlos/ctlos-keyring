# Ctlos keyring gpg-key

pkgname=ctlos-keyring
pkgver=$(date +%Y%m%d)
pkgrel=2
pkgdesc='ctlos PGP keyring'
arch=('any')
url='https://github.com/ctlos/ctlos-keyring'
license=('GPL')
install="${pkgname}.install"
source=('Makefile'
        'ctlos.gpg'
        'ctlos-revoked'
        'ctlos-trusted')
sha256sums=('SKIP'
            'SKIP'
            'SKIP'
            'SKIP')

package() {
  cd "${srcdir}"
  make PREFIX=/usr DESTDIR=${pkgdir} install
}
