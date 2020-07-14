# Ctlos keyring gpg-key

pkgbase=ctlos-keyring
pkgname=("$pkgbase")
destdir=/usr/share/pacman/keyrings
pkgver=$(date +%Y%m%d)
pkgrel=7
pkgdesc="Ctlos keyring"
arch=('any')
url="https://github.com/ctlos"
license=('GPL3')
source=("https://github.com/ctlos/ctlos-keyring/raw/master/ctlos-keyring.install"
        "https://github.com/ctlos/ctlos-keyring/raw/master/ctlos.gpg")

sha256sums=('SKIP'
            'SKIP')

install=$pkgbase.install

package() {
    mkdir -p ${pkgdir}/$destdir
    cd ..
    mv ctlos.gpg ${pkgdir}/$destdir
    install -dm 755 "${pkgdir}/$destdir"

}
