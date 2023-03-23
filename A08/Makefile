CC=gcc
% :: %.c
	$(CC) -g -Wall -Wvla -Werror $< -o $@ -lm

all: single_mandelbrot multi_mandelbrot warmup search

single_mandelbrot: single_mandelbrot.c read_ppm.c write_ppm.c
	$(CC) -g -Wall -Wvla -Werror -Wno-unused-variable single_mandelbrot.c read_ppm.c write_ppm.c -o $@ -lm

multi_mandelbrot: multi_mandelbrot.c read_ppm.c write_ppm.c
	$(CC) -g -Wall -Wvla -Werror -Wno-unused-variable multi_mandelbrot.c read_ppm.c write_ppm.c -o $@ -lm

clean: 
	rm single_mandelbrot multi_mandelbrot search warmup

