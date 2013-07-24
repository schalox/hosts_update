# Contributor: graysky <graysky AT archlinux dot us>
# Contributor: schalox <schalox at gmail dot com>
_upstream=hosts_update
pkgname=hosts_update_schalox
pkgver=0.0.0
pkgrel=1
pkgdesc='Updates /etc/hosts with the mvps blocklist to prevent thousands of parasites, hijackers and unwanted adware/spyware/privacy websites from working.'
arch=('any')
depends=()
license=('GPL')
provides=("$_upstream")
conflicts=("$_upstream")
replaces=("$_upstream")
url=("https://github.com/schalox/${_upstream}")
backup=('etc/hosts.local')
source=('git://github.com/schalox/hosts_update.git')
sha256sums=('SKIP')

pkgver() {
    date '+%Y%m%d'
}

package() {
    cd "$_upstream"
    install -Dm755 "$_upstream" "$pkgdir/usr/bin/$_upstream"
    install -Dm644 hosts.local "$pkgdir/etc/hosts.local"
    install -Dm644 service "$pkgdir/usr/lib/systemd/system/${_upstream}.service"
}
