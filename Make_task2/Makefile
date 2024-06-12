CC = gcc

all: main

main: main.o src1.o src2.o src3.o
	$(CC) -o $@ $^

main.o: main.c
	$(CC) -c $< -o $@

include src1.mk
include src2.mk
include src3.mk

clean:
	rm -f *.o main

.PHONY: clean
