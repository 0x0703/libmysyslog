Лекционная практика №2
В консоли выполняем команду make all
После успешной сборки прописываем команду sudo nano /etc/ld.so.conf
Дописать в файл пути /home/username/mysyslog/libmysyslog /home/username/mysyslog/libmysyslog-text /home/username/mysyslog/libmysyslog-json
Выполнить команду sudo ldconfig
Далее запускаем демона и клиента командами sudo make run-daemon или run-client
В окне активного клиента прописываем путь до файла с логами /var/log/mysyslog.log# libmysyslog
