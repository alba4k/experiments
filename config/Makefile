CC := clang
CFLAGS := -Wall -Wextra -O3 -march=native

build: main.o config.o
	clang -o build main.o config.o $(CFLAGS)

main.o: main.c config.h
	clang -c main.c $(CFLAGS)

pickle.o: config.c config.h
	clang -c config.c $(CFALGS)

run: build
	./build

clean:
	-rm -rf build *.o