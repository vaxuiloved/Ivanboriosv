# Ivanborisov
sudo apt install postgresql postgresql-contrib -y
git clone 
cd opendlp
make
sudo make install

# Создание БД и пользователя для OpenDLP
sudo -u postgres psql -c "CREATE DATABASE opendlp;"
sudo -u postgres createuser opendlp_user
sudo -u postgres psql -d opendlp -c
