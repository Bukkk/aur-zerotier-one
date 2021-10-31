pkgname=zerotier-one-s6
pkgver=2021031
pkgrel=1
pkgdesc="s6-rc service scripts for zerotier-one"
arch=('any')
url="https://github.com/Bukkk/s6-services"
license=('GPL')
groups=('s6-system')
provides=('init-zerotier-one')
conflicts=('init-zerotier-one')
depends=('zerotier-one' 's6-base')
makedepends=('git')
backup=('etc/s6/config/zerotier-one.conf')
source=("git+https://github.com/Bukkk/s6-services.git")
sha256sums=('SKIP')

package() {
    cd "${srcdir}"/s6-services
    sh install.sh "zerotier-one" "${pkgdir}"
}

