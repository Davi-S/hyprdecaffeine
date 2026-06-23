# Maintainer: Davi Alves Sampaio <davialvessampaio00@gmail.com>
pkgname=decaf
pkgver=1.0.3
pkgrel=1
pkgdesc="A Rofi-based sleep timer utility"
arch=('any')
url="https://github.com/davi-s/decaf"
license=('MIT')
depends=('bash' 'systemd' 'rofi' 'libnotify')
# This downloads the source code directly from your GitHub release
source=("$pkgname-$pkgver.tar.gz::https://github.com/davi-s/decaf/archive/refs/tags/${pkgver}.tar.gz")
sha256sums=('SKIP') # Remember to run updpkgsums or makepkg -g to update this

package() {
    cd "$pkgname-$pkgver"

    # Install the script directly to /usr/bin
    install -Dm755 src/decaf "$pkgdir/usr/bin/decaf"
}
