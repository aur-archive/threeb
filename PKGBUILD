pkgname=threeb
pkgver=1.1
pkgrel=1
pkgdesc="3B Microscopy Analysis Software-Bayesian analysis of blinking and bleaching, analyses data in which many overlapping fluorophores undergo bleaching and blinking events, giving the structure at enhanced resolution,using a Hidden Markov Model (HMM)."
arch=('x86_64' 'i686')

license=('GPLv3')
depends=('toon' 'libcvd' 'gvars3')
optdepends=()
makedepends=('gcc' 'make')
conflicts=()
replaces=()
backup=()
#options=(!strip)
url=("http://www.coxphysics.com/3b/")
source=("http://coxphysics.com/3b/threeB-${pkgver}.tar.gz")
md5sums=('b75cbe9ef880bf1d9c5ab2f2ccddbe5f')


build() {
  cd "${srcdir}/threeB-${pkgver}"
  export
  ./configure --prefix=/usr   
  make
}
 
package() {
  cd "${srcdir}/threeB-${pkgver}"
  mkdir -p "${pkgdir}/usr/bin"
  cp multispot5_headless "${pkgdir}/usr/bin"
}

