# rvm-install-ubuntu-16.04

gpg2 --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3
curl -L https://get.rvm.io | bash -s stable
source ~/.rvm/scripts/rvm
rvm install 2.2.0
rvm use 2.2.0 --default
ruby -v
gem install bundler
