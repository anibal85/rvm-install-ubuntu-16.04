# rvm-install-ubuntu-16.04

gpg2 --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3
curl -L https://get.rvm.io | bash -s stable
source ~/.rvm/scripts/rvm
rvm install 2.2.0
rvm use 2.2.0 --default
ruby -v
gem install bundler


Asegúrese de que estén instalados curl y gpg, así como una cadena de herramientas del compilador.

Curl y gpg son necesarios para más pasos de instalación, mientras que la cadena de herramientas del compilador es necesaria para instalar gemas comunes de Ruby.



