CC = gcc
CFLAGS = -Wall -g -I/home/kali/mysyslog/libmysyslog -I/home/kali/mysyslog/libmysyslog-text -I/home/kali/mysyslog/libmysyslog-json
LDFLAGS = -L/home/kali/mysyslog/libmysyslog -L/home/kali/mysyslog/libmysyslog-text -L/home/kali/mysyslog/libmysyslog-json -lmysyslog -lmysyslog-text -lmysyslog-json

all: libmysyslog-client

libmysyslog-client: libmysyslog-client.o
	$(CC) -o $@ $^ $(LDFLAGS)

libmysyslog-client.o: libmysyslog-client.c
	$(CC) $(CFLAGS) -c $<

run: libmysyslog-client
	./libmysyslog-client

clean:
	rm -f libmysyslog-client *.o
