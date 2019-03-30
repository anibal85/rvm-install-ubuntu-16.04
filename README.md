# rvm-install-ubuntu-16.04

Instalando RVM y Ruby

gpg2 --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3
curl -L https://get.rvm.io | bash -s stable
source ~/.rvm/scripts/rvm
rvm install 2.2.0
rvm use 2.2.0 --default
ruby -v
gem install bundler


Asegúrese de que estén instalados curl y gpg, así como una cadena de herramientas del compilador.

Curl y gpg son necesarios para más pasos de instalación, mientras que la cadena de herramientas del compilador es necesaria para instalar gemas comunes de Ruby.

Instalando RVM y Ruby

RVM automatiza el proceso de configuración de un entorno Ruby en su sistema Ubuntu. Vamos a instalarlo para que podamos usarlo para instalar Ruby.

La forma más rápida de instalar Ruby con RVM es ejecutar el script de instalación alojado en el sitio web de RVM.

Primero, use el gpgcomando para ponerse en contacto con un servidor de claves públicas y solicite la clave del proyecto RVM que se utiliza para firmar cada versión de RVM. Esto le permite verificar la legitimidad de la versión RVM que descargará. Desde su directorio de inicio, ejecute el siguiente comando:

gpg --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3 7D2BAF1CF37B13E2069D6956105BD0E739499BDB


Lo utilizaremos curlpara descargar el script de instalación de RVM. Instalar curlsi no está ya instalado.

sudo apt-get install curl

