# Maintainer: Jakob Wadsager <jakobw@archlinux.org>
# Contributer: Rob Lass <firstname dot lastname at gmail dot com>

pkgname=python2-qstk
pkgver=0.2.8
pkgrel=1
pkgdesc="QuantSoftware ToolKit"
arch=('i686' 'x86_64')
url="http://wiki.quantsoftware.org/index.php?title=QuantSoftware_ToolKit"
license=('New BSD')
conflicts=()
provides=()
depends=('python2>2.7'
  'python2-numpy>=1.6.1'
  'python2-scipy>=0.9.0'
  'python2-matplotlib>=1.1.0'
  'python2-pandas>=0.7.3'
  'python2-dateutil>=1.5'
  'python2-cvxopt>=1.1.3'
  'python2-scikit-learn>=0.11')
source=(http://pypi.python.org/packages/source/Q/QSTK/QSTK-${pkgver}.tar.gz)
md5sums=('bac816724bcb6eebd5dbb09e43166815')

build() {
  cd "$srcdir/QSTK-$pkgver"
  python2 setup.py build

}

package() {
  cd "$srcdir/QSTK-$pkgver"
  python2 setup.py install --root="$pkgdir/" --optimize=1
}
