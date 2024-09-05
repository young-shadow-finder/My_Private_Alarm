CC = g++
CFLAGS = -Wall -g
LDFLAGS = -lstdc++

SRCS := $(wildcard lib/*.cpp)
SRCS += $(wildcard *.cpp)

OBJS := $(SRCS:.cpp=.o)

TARGET := main

all: $(TARGET)

$(TARGET): $(OBJS)
	$(CC) $(LDFLAGS) -o $@ $^

%.o: %.cpp
	$(CC) $(CFLAGS) -c -o $@ $<

clean:
	rm -f $(TARGET) $(OBJS)