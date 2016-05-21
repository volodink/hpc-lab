all: clean prepare build

clean:
	rm -rf bin
	rm -rf docs
	rm -rf bench/data
	
prepare:
	mkdir bin
	mkdir bench/data
build:
	gcc -Wall -O3 -pedantic -pedantic-errors -o bin/test src/main.c

run:
	./bin/test
	
doc:
	doxygen

bench:
	./bin/test > bench/data/data.txt
	python bench_plot.py
