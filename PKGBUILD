# Ctlos keyring gpg-key

pkgname=ctlos-keyring
pkgver=stable
pkgrel=1
pkgdesc='ctlos PGP keyring'
arch=('x86_64')
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
