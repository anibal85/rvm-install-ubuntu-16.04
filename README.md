# rvm-install-ubuntu-16.04

Instalando RVM y Ruby

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

-------------------Instalacion---------------------------

gpg2 --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3 7D2BAF1CF37B13E2069D6956105BD0E739499BDB
 Instalacion de Keys en Linux 
 
 ## Instalar Curl si no esta instalado 
 
 apt-get install curl
 
 \curl -sSL https://get.rvm.io | bash -s stable
 
 # Comando para Listar paquete y ver version de RVM
 rvm -v
 rvm list known 
 
  # Instalacion cualquier Version de Ruby
 rvm install 2.3.4
 
 # Ver paquetes instalados en RVM 
 rvm list
 
 # Comando para Cambiar de versiones 
 rvm use version_ruby
