pkgname='python-fontconfig'
pkgver='0.5.0'
pkgrel=3
pkgdesc='Python bindings for Fontconfig library'
arch='any'
url='https://github.com/Vayn/python-fontconfig'
license='GPL3'
makedepends=('cython')
depends=('python' 'fontconfig')
source=("$pkgname-$pkgver.tar.gz::https://github.com/Vayn/python-fontconfig/archive/v$pkgver.tar.gz")

package() {
    cd $srcdir/$pkgname-$pkgver
    python setup.py build_ext -i
    python setup.py install --prefix=$pkgdir/usr
}

md5sums=('82a818565d0507dd85b994987c7749b8')
