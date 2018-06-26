CC=riscv64-unknown-elf-gcc
CFLAGS= -std=gnu++11 -O0 -g3 -DTIME
LFLAGS= -std=gnu++11 -O0 -g3 -static

all:
	$(CC) -c $(CFLAGS) dhry_1.c -o dhry_1.o
	$(CC) -c $(CFLAGS) dhry_2.c -o dhry_2.o

	$(CC) -o main *.o $(LFLAGS)

run:
	qemu-riscv64 ./main

clean:
	rm -rf main *.o
