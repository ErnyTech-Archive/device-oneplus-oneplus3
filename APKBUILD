# Reference: <https://postmarketos.org/devicepkg>
pkgname="device-oneplus-oneplus3"
pkgdesc="OnePlus 3/3T"
pkgver=0.1
pkgrel=0
url="https://postmarketos.org"
license="MIT"
arch="aarch64"
options="!check !archcheck"
depends="postmarketos-base linux-oneplus-oneplus3 mkbootimg mesa-dri-swrast mdss-fb-init-hack"
makedepends="devicepkg-dev"
source="deviceinfo fb.modes"

build() {
	devicepkg_build $startdir $pkgname
}

package() {
	devicepkg_package $startdir $pkgname
	install -Dm644 "$srcdir"/fb.modes "$pkgdir"/etc/fb.modes
}


sha512sums="9e100b4289b5e5c6698ffd38a8898b577eca4bc75fdb88afff63bac024d461a540c40d48cb64f6b6a5a7812e3d2e5bd42c4f9cf493e18c860daceffdb0e9dbad  deviceinfo"
