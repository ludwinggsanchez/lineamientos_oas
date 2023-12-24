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