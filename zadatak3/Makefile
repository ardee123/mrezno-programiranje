TCPKLIJENT=tcpklijent
TCPSERVER=tcpserver

SOURCE_TCPSERVER=tcpserver.c

SOURCE_TCPKLIJENT=tcpklijent.c

CFLAGS=-Wall -g

OBJECTS_TCPSERVER=${SOURCE_TCPSERVER:.c=.o}
OBJECTS_TCPKLIJENT=${SOURCE_TCPKLIJENT:.c=.o}

$(TCPSERVER) $(TCPKLIJENT): $(OBJECTS_TCPSERVER) $(OBJECTS_TCPKLIJENT)
	$(CC) $(OBJECTS_TCPSERVER) -o $(TCPSERVER)
	$(CC) $(OBJECTS_TCPKLIJENT) -o $(TCPKLIJENT)
	
	
$(OBJECTS_TCPSERVER): $(HEADERS_TCPSERVER)
$(OBJECTS_TCPKLIJENT): $(HEADERS_TCPKLIJENT)

clean:
	-rm -f $(TCPSERVER) $(TCPKLIJENT) $(OBJECTS_TCPSERVER) $(OBJECTS_TCPKLIJENT) *.core
