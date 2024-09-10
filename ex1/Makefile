demo: main.o thing1.o thing2.o
	g++ main.o thing1.o thing2.o -o demo

#If we change anything in the header files we want to recompile main.o
main.o: main.cpp thing1.h thing2.h 
	g++ -c main.cpp

thing1.o: thing1.cpp thing1.h 
	g++ -c thing1.cpp

thing2.o: thing2.cpp thing2.h 
	g++ -c thing2.cpp

run: demo
	./demo

