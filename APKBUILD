# Contributor: Natanael Copa <ncopa@alpinelinux.org>
# Maintainer: Natanael Copa <ncopa@alpinelinux.org>
pkgname=alpine-base
pkgver=2.6.0_rc3
pkgrel=0
pkgdesc="Meta package for minimal alpine base"
url="http://alpinelinux.org"
arch="noarch"
license="GPL"
depends="alpine-baselayout alpine-conf apk-tools busybox busybox-initscripts
	openrc libc-utils alpine-keys"
makedepends=
install=
subpackages=
replaces="alpine-baselayout"
source=""

build() {
	return 0
}

package() {
	mkdir -p "$pkgdir"/etc
	# create /etc/alpine-release
	echo $pkgver > "$pkgdir"/etc/alpine-release

	# create /etc/issue
	cat >"$pkgdir"/etc/issue<<EOF
Welcome to Alpine Linux ${pkgver%.*}
Kernel \\r on an \\m (\\l)

EOF
}

