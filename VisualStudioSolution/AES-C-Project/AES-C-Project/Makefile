CFLAGS := -ggdb -Wall -O2

aes.o: aes_core.c aes_locl.h aes.h
	gcc $(CFLAGS) -c $< -o $@

test: main_test.c aes.o
	gcc $(CFLAGS) $^ -o $@

.PHONY: clean
clean:
	rm -f *.o test
