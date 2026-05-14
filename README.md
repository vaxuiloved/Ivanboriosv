# Ivanborisov
Установка и настройка MS SQL Server 2022 
# Обновление системы
sudo apt update && sudo apt upgrade -y

# Импорт ключа и добавление репозитория
wget -qO- https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
sudo add-apt-repository "$(wget -qO- https://packages.microsoft.com/config/ubuntu/22.04/mssql-server-2022.list)"

# Установка SQL Server
sudo apt install mssql-server -y
sudo /opt/mssql/bin/mssql-conf setup  #

# Проверка статуса
sudo systemctl status mssql-server   active 
