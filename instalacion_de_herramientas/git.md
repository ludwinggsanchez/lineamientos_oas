# Instalación Git

## Instalación Git descargable

1. Ingresar a [https://git-scm.com/download/win](https://git-scm.com/download/win) y buscar la version deseada de git

## Instalación Git código fuente

### Requerimientos

1. Para instalar Git desde el código fuente es necesario tener las siguientes librerías de las que Git depende: curl, zlib, openssl, expat y libiconv.

#### Sistema con yum

```bash
yum install curl-devel expat-devel gettext-devel \
  openssl-devel zlib-devel
```

#### Sistema con apt-get

```bash
apt-get install libcurl4-gnutls-dev libexpat1-dev gettext \
  libz-dev libssl-dev
```
2. Se debe descargar la versión más reciente de Git
[https://www.kernel.org/pub/software/scm/git](https://www.kernel.org/pub/software/scm/git) o [https://github.com/git/git/releases](https://github.com/git/git/releases)

3. compilar e instalar de la siguiente manera:

```bash
tar -zxf git-2.0.0.tar.gz
cd git-2.0.0
make configure
./configure --prefix=/usr
make all doc info
sudo make install install-doc install-html install-info
```

4. una vez terminado se puede obtener Git a través de Git para mantener las actualizaciones

```bash
git clone git://git.kernel.org/pub/scm/git/git.git
```
