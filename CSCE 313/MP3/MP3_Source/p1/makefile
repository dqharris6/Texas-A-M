# makefile

all: dataserver client

reqchannel.o: reqchannel.h reqchannel.cpp
	g++ -c -g reqchannel.cpp

dataserver: dataserver.cpp reqchannel.o 
	g++ -o dataserver dataserver.cpp reqchannel.o -lpthread

client: client.cpp reqchannel.o
	g++ -o client client.cpp reqchannel.o
