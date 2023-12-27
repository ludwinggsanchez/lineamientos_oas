# Instalación Golang

1. Descargar código fuente de [https://golang.org/dl/](https://golang.org/dl/)
```bash
cd Downloads/
sudo tar -C /usr/local -xzf go1*.tar.gz
```

2. Configurar variables de entorno
```bash
sudo nano /etc/profile.d/goenv.sh
```
Agregar al archivo lo siguiente
```bash
export GOROOT=/usr/local/go
export GOPATH=$HOME/go
export PATH=$PATH:$GOROOT/bin:$GOPATH/bin
```

3. Actualizar variables de entorno
```bash
source /etc/profile.d/goenv.sh
```

4. Crear directorio de trabajo
```bash
mkdir -p  ~/go
```

5. Comprobar instalacion
```bash
go version
echo $GOPATH
cd $GOPATH
```

## Manjaro

1. instalar go
```zsh
sudo pacman -S go
```

2. Configurar variables de entorno

```zsh
export GOROOT=/usr/lib/go
export GOPATH=$HOME/go
export PATH=$PATH:$GOROOT/bin:$GOPATH/bin
```

3. Crear directorio de trabajo
```bash
mkdir -p  ~/go
```

4. Comprobar instalacion
```bash
go version
echo $GOPATH
cd $GOPATH
```

## Windows

1. Descargar el instalador de windows [CLICK AQUI](https://go.dev/dl/)
2. Durante el proceso de instalación, se ofrece la opción de incorporar Go al PATH del sistema y configurar las variables de entorno de manera automática. Es recomendable seleccionar estas opciones para garantizar que Go esté accesible desde cualquier ubicación en el sistema.
3. Las variables de entorno están configuradas automáticamente para el usuario actual. Para hacer esta configuración genérica y aplicable a todos los usuarios, es necesario configurar las variables de entorno a nivel de sistema y actualizar el PATH correspondientemente.