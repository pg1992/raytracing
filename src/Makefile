render.ppm: main.elf
	./main.elf >render.ppm

main.elf: main.cc vec3.h ray.h color.h hittable.h sphere.h
	g++ -Wall -Wextra -Weffc++ -Wpedantic -std=c++23 -o main.elf main.cc

.PHONY: clean
clean:
	rm -rf *.elf *.ppm *.o *.out
