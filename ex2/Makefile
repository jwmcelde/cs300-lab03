CXX = g++
OBJECTS = thing1.o main.o thing2.o
FLAGS = -std=c++20

demo: $(OBJECTS)
	$(CXX) $(FLAGS) $(OBJECTS) -o demo

#If we change anything in the header files we want to recompile main.o
main.o: main.cpp thing1.o thing2.o
	$(CXX) -c main.cpp

thing1.o: thing1.cpp thing1.h 
	$(CXX) -c thing1.cpp

thing2.o: thing2.cpp thing2.h 
	$(CXX) -c thing2.cpp

run: demo
	./demo

