# Maintainer: Patrick Ulbrich <zulu99 at gmx . net>

pkgname=mailnag-gnome-shell
pkgver=3.12.0
pkgrel=1
pkgdesc="Mailnag GNOME-Shell extension."
arch=('any')
url="https://github.com/pulb/mailnag-gnome-shell"
license=('GPL')
depends=('mailnag>=0.9', 'folks')
makedepends=('vala')
source=('https://github.com/pulb/mailnag-gnome-shell/archive/v3.12.0.tar.gz')
md5sums=('b40d9f25a4932094b2fd5870f8029744')
install='mailnag-gnome-shell.install'

build() {
	cd ${srcdir}/${pkgname}-${pkgver}
	make
}

package() {
	cd ${srcdir}/${pkgname}-${pkgver}
	make prefix="$pkgdir" install
 	install -D -m644 LICENSE "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}