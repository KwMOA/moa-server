CPLUS_INCLUDE_PATH = /usr/local/boost_1_62_0:../../../Lib/ExternalLib/tinyxml2:../../../Lib/ServerNetworkLib:../../Packet
export CPLUS_INCLUDE_PATH

VPATH = ../../../Lib/ExternalLib/tinyxml2 ../../../Lib/ServerNetworkLib ../../Packet .

OBJECTS = tinyxml2.o Log.o WorkerThread.o Network.o IOManager.o ServerInfo.o FrontData.o FrontServer.o User.o main.o

FrontServer : $(OBJECTS)
g++ -g -rdynamic -o $@ $^ -L/usr/local/boost_1_62_0/stage/lib -lz -lboost_filesystem -lboost_system -I/usr/local/uuid

clean:
rm -rf *.o FrontServer
