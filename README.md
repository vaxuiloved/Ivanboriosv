# Ivanborisov
#!/ Обновление системы
sudo apt update && sudo apt upgrade -y

# Импорт GPG‑ключа Microsoft
wget -qO-  | sudo apt-key add -

# Добавление репозитория SQL Server
sudo add-apt-repository "$(wget -qO- 
# Установка SQL Server
sudo apt install mssql-server -y

# Запуск скрипта настройки
sudo /opt/mssql/bin/mssql-conf setup

# Проверка статуса службы
sudo systemctl status mssql-server
