all: clean prepare build

clean:
	rm -rf bin
	rm -rf docs
	
prepare:
	mkdir bin
	
build:
	gcc -Wall -O3 -pedantic -pedantic-errors -o bin/test src/main.c

run:
	./bin/test
	
doc:
	doxygen

