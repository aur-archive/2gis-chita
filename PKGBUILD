pkgname=2gis-chita
pkgver=8
pkgrel=1
pkgdesc="Map of Chita for 2GIS, December 2012"
arch=('i686' 'x86_64')
url="http://chita.2gis.ru/how-get/linux/"
license=('custom')
depends=('2gis>=3.12.0.2')
source=("http://download.2gis.ru/arhives/2GISData_Chita-8.orig.zip")
md5sums=('faf4f59a254ca4844baec014d73d6281')

build() {
  cd $startdir
# Installing to /opt/2gis
  install -D -m 644 ${startdir}/src/2gis/3.0/Data_Chita.dgdat "${startdir}/pkg/opt/2gis/chita.dgdat" || return 1
  install -D -m 644 ${startdir}/src/2gis/3.0/Plugins/DGisLan/Chita.dglf "${startdir}/pkg/opt/2gis/Plugins/DGisLan/Chita.dglf" || return 1
}
