


CXX = g++
OBJECTS = thing1.o main.o thing2.o
FLAGS = -std=c++20
SOURCE = $(wildcard *.cpp)

demo: $(OBJECTS)
	$(CXX) $(FLAGS) $(OBJECTS) -o demo

# $< refers to the first prequisite
# $@ refers to the target
%.o: %.cpp %.h
	$(CXX) -c $< -o $@

run: demo
	./demo

echo:
	echo $(SOURCE)

clean: 
	rm -f *.o demo
