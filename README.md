Лекционная практика №2
1.В консоли выполняем команду make all
2.После успешной сборки прописываем команду sudo nano /etc/ld.so.conf
3.Дописать в файл пути /home/username/mysyslog/libmysyslog /home/username/mysyslog/libmysyslog-text /home/username/mysyslog/libmysyslog-json
4.Выполнить команду sudo ldconfig
5.Далее запускаем демона и клиента командами sudo make run-daemon или run-client
6.В окне активного клиента прописываем путь до файла с логами /var/log/mysyslog.log# libmysyslog
