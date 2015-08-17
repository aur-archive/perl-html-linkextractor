# Maintainer: Brian Parsons <brian@pmex.com>
#

_author="PODMASTER"
_perlmod="HTML::LinkExtractor"
pkgname=perl-html-linkextractor
pkgver=0.13
pkgrel=1
pkgdesc="Extract links from an HTML document"
arch=('any')
url="http://search.cpan.org/dist/HTML-LinkExtractor/"
license=('GPL' 'PerlArtistic')
depends=('perl')
options=('!emptydirs')
source=("http://search.cpan.org/CPAN/authors/id/P/PO/PODMASTER/HTML-LinkExtractor-${pkgver}.tar.gz")
md5sums=('a30143b35ef76576fb984696746776de')

build () {

	cd ${srcdir}/HTML-LinkExtractor-${pkgver}
	PERL_MM_USE_DEFAULT=1 perl Makefile.PL INSTALLDIRS=vendor
	make

}

package() {

	cd ${srcdir}/HTML-LinkExtractor-${pkgver}
	make DESTDIR=${pkgdir} install

}
