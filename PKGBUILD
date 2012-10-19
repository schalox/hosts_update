# Contributor: graysky <graysky AT archlinux dot us>
# Contributor: schalox <schalox at gmail dot com>
pkgname=hosts_update
pkgver=1.0
pkgrel=3
pkgdesc='Updates /etc/hosts with the mvps blocklist to prevent thousands of parasites, hijackers and unwanted adware/spyware/privacy websites from working.'
arch=('any')
depends=()
license=('GPL')
url=("https://github.com/schalox/hosts_update")
source=("hosts_update" "hosts.local" "service")
backup=('etc/hosts.local')

package() {
    install -Dm755 "$pkgname" "$pkgdir/usr/bin/$pkgname"
    install -Dm644 hosts.local "$pkgdir/etc/hosts.local"
    install -Dm644 service "$pkgdir/usr/lib/systemd/system/$pkgname.service"
}
sha256sums=('667e3d8c30d92bc88d7ecf5fe230e8c3c4db4a6e2d2d2e3bcbbca799f3c35865'
            'b45d87fbfbdf5e4cecaa8afc807e760fc5fdf7ed2423338ea98f6c7730881d89'
            '95b73c0856ab80a14c0a7637a68a6c551484fbc95ea6b2e87d4edf3d773d2e21')
