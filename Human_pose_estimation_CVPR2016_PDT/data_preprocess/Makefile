CC = gcc
CXX = g++ -O3
OPT = -std=c++0x
BOOST_ROOT = /usr/local
INC = -I$(BOOST_ROOT)/include
LDFLAGS = -L$(BOOST_ROOT)/lib
LDFLAGS += -lboost_system -lboost_filesystem

all: preprocess_pdt_db.cpp
	$(CXX) $(OPT) -o out preprocess_pdt_db.cpp $(INC) $(LDFLAGS) `pkg-config --cflags --libs opencv`
