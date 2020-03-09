pkgname=ctlos-keyring
pkgver=0.3
pkgrel=1
pkgdesc='Ctlos PGP keyring'
arch=('any')
url='https://github.com/ctlos/ctlos-keyring'
license=('GPL')
install="${pkgname}.install"
source=('Makefile'
        'ctlos.gpg'
        'ctlos-trusted')
sha256sums=('fd85add03d59682c179a6ed91c181532637a8bbc831be0e2050e38f204bac228'
            'f6a9fb4a1eecfe74995dd4e851fcf66984cf42a1c3cf440e78c16f2727a41c9c'
            '0d46a9bd4843e59705f3b7209744851157c59e4f715b3f86dd86ded9a203db6b')

package() {
  cd "${srcdir}"
  make PREFIX=/usr DESTDIR=${pkgdir} install
}
# -*- mode: bash;-*-
