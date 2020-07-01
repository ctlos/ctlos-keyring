# Ctlos keyring gpg-key

pkgbase=ctlos-keyring
pkgname=("$pkgbase")
destdir=/usr/share/pacman/keyrings
pkgver=$(date +%Y%m%d)
pkgrel=3
pkgdesc="Ctlos keyring"
arch=('any')
url="https://github.com/ctlos"
license=('GPL3')
install=$pkgbase.install

source=('Makefile'
        'ctlos.gpg'
        'ctlos-revoked'
        'ctlos-trusted')
sha256sums=('3155bfa755a3c67f5aca51513d4231f372a21daed6e5c750e8ac24a5f1775a57'
            'e0218abb96467c350944757838e2a57bb0e28142d2c08aa79870df2f68204968'
            'e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855'
            '0d46a9bd4843e59705f3b7209744851157c59e4f715b3f86dd86ded9a203db6b')

package() {
  cd "${srcdir}"
  make PREFIX=/usr DESTDIR=${pkgdir} install
}

