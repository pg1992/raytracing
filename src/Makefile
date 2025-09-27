CXX=g++
CXXFLAGS=-Wall -Wextra -Wpedantic -std=c++23

HEADERS=vec3.h ray.h color.h hittable.h sphere.h camera.h material.h

render.ppm: main.elf
	./main.elf >render.ppm

main.elf: main.cc $(HEADERS)
	$(CXX) $(CXXFLAGS) -o $@ main.cc

.PHONY: clean
clean:
	rm -rf *.elf *.ppm *.o *.out
