pkgname=shellcheck
pkgver=0.11.0
pkgrel=1
pkgdesc='ShellCheck, a static analysis tool for shell scripts'
arch=('x86_64')
url='https://www.shellcheck.net/'
license=('GPL3')

depends=(bash)
optdepends=('nodejs: To install and run bash-language-server')

install=${pkgname}.install

source=("https://github.com/koalaman/${pkgname}/releases/download/v${pkgver}/shellcheck-v${pkgver}.linux.${arch}.tar.xz")

sha256sums=('8c3be12b05d5c177a04c29e3c78ce89ac86f1595681cab149b65b97c4e227198')

package() {
    cd "${srcdir}/${pkgname}-v${pkgver}"
    install -Dm755 "${pkgname}" "${pkgdir}/usr/bin/shellcheck"
    install -Dm644 "LICENSE.txt" "${pkgdir}/usr/share/licenses/LINCENSE.txt"
}
