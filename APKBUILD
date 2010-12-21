# Contributor: Natanael Copa <ncopa@alpinelinux.org>
# Maintainer: Natanael Copa <ncopa@alpinelinux.org>
pkgname=alpine-base
pkgver=2.1.0_git20101221
pkgrel=0
pkgdesc="Meta package for minimal alpine base"
url="http://alpinelinux.org"
arch="x86 x86_64"
license="GPL"
depends="alpine-baselayout alpine-conf apk-tools busybox busybox-initscripts
	openrc bbsuid"
[ "$ALPINE_LIBC" != "eglibc" ] && depends="$depends uclibc-utils"
makedepends=
install=
subpackages=
source="http://dev.alpinelinux.org/~ncopa/alpine/alpine-devel@lists.alpinelinux.org-4a6a0840.rsa.pub
	http://nenolod.net/~nenolod/alpine-keys/alpine-devel@lists.alpinelinux.org-4d07755e.rsa.pub
	"

build() {
	return 0
}

package() {
	mkdir -p "$pkgdir"/etc/apk/keys
	install -m644 "$srcdir"/*.pub "$pkgdir"/etc/apk/keys/
	echo $pkgver > "$pkgdir"/etc/alpine-release
}
md5sums="75ee19ea2b03c12bc171647edc677f6f  alpine-devel@lists.alpinelinux.org-4a6a0840.rsa.pub
ca7d06006181b625cf1ff4aefd51bd08  alpine-devel@lists.alpinelinux.org-4d07755e.rsa.pub"
