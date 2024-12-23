CC = gcc
CFLAGS = -Wall -g -I/home/kali/mysyslog/libmysyslog -I/home/kali/mysyslog/libmysyslog-text -I/home/kali/mysyslog/libmysyslog-json
LDFLAGS = -L/home/kali/mysyslog/libmysyslog -L/home/kali/mysyslog/libmysyslog-text -L/home/kali/mysyslog/libmysyslog-json -lmysyslog -lmysyslog-text -lmysyslog-json
all: libmysyslog-daemon

libmysyslog-daemon: libmysyslog-daemon.o
	$(CC) -o $@ $^ $(LDFLAGS)

libmysyslog-daemon.o: libmysyslog-daemon.c
	$(CC) $(CFLAGS) -c $<

run: libmysyslog-daemon
	./libmysyslog-daemon

clean:
	rm -f libmysyslog-daemon *.o
