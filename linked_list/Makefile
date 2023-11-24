CC := clang
CFLAGS := -Wall -Wextra -O3 -march=native

build: main.o linked_list.o
	clang -o build main.o linked_list.o $(CFLAGS)

main.o: main.c linked_list.h
	clang -c main.c $(CFLAGS)

pickle.o: pickle.c pickle.h
	clang -c pickle.c $(CFALGS)

run: build
	./build

clean:
	-rm -rf build *.o