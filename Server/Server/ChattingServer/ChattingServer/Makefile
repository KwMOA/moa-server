CPLUS_INCLUDE_PATH = /usr/local/boost_1_62_0:../../../Lib/ExternalLib/tinyxml2:../../../Lib/ServerNetworkLib:../../Packet
export CPLUS_INCLUDE_PATH

VPATH = ../../../Lib/ExternalLib/tinyxml2 ../../../Lib/ServerNetworkLib ../../Packet .

OBJECTS = tinyxml2.o Log.o WorkerThread.o Network.o IOManager.o LObject.o ChattingData.o ChattingServer.o User.o main.o

ChattingServer : $(OBJECTS)
g++ -g -rdynamic -o $@ $^ -L/usr/local/boost_1_62_0/stage/lib -I/usr/local/uuid -lz -lboost_filesystem -lboost_system -lpthread

clean:
rm -rf *.o ChattingServer
