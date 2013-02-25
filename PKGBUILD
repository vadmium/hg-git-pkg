_proj=hg-git
pkgname="$_proj"
pkgver=0.3.4
pkgrel=1
pkgdesc="Mercurial plugin to convert to and from a Git repository"
arch=(any)
url="http://$_proj.github.com"
license=(GPL2)
depends=(mercurial python-dulwich)

_rls="$_proj-$pkgver"
source+=(
"https://pypi.python.org/packages/source/${_proj:0:1}/$_proj/$_rls.tar.gz")
md5sums+=(a2a34f60dd5ce66ba9015caa70f3f7e9)

package() {
    cd "$srcdir/$_rls"
    python2 setup.py install --root="$pkgdir" --optimize=1
}
