pkgname=custom-openrc
pkgver=0.0.1
pkgrel=1
pkgdesc="OpenRC init scripts"
arch=('any')
url=""
optdepends=(
'openrc'
'mpd'
'mympd'
'openlist'
'qbittorrent-nox'
'snapcast'
'aria2'
'surge'
'transmission'
)
conflicts=(
'custom-mpd-openrc'
'mpd-openrc'
'mympd-openrc'
'openlist-openrc'
'qbittorrent-nox-openrc'
'snapcast-openrc'
'mihomo-openrc'
'aria2-openrc'
'surge-openrc'
'transmission-openrc'
)
license=('GPL')

package () {
    mkdir -p "$pkgdir/etc/user/init.d/"
    cd $srcdir
    for i in *; do
        install -m755 "$srcdir/$i" "$pkgdir/etc/user/init.d/$i"
    done
}
