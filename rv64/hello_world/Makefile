CC=riscv64-unknown-elf-c++
CFLAGS= -std=gnu++11 -O0 -g3
LFLAGS= -std=gnu++11 -O0 -g3 -static

all:
	$(CC) -c $(CFLAGS) main.cpp  -o main.o

	$(CC) -o main *.o $(LFLAGS)

run:
	qemu-riscv64 ./main

clean:
	rm -rf main *.o
