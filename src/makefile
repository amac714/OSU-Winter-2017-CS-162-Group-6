
CXX = g++

CXXFLAGS = -std=c++0x

#DEBUG flags
#CXXFLAGS += -Wall
#CXXFLAGS += -pedantic-errors
#CXXFLAGS += -g

LDFLAGS =

OBJS = main.o

# For Windows
LIBS = menu_library/douglbre_util.obj

# For Linux
#LIBS = menu_library/douglbre_util.o

SRCS = main.cpp

HEADERS = menu_library/douglbre_util.hpp

EXECUTABLE = main

main: $(OBJS) $(HEADERS)
	$(CXX) $(LDFLAGS) $(OBJS) $(LIBS) -o $(EXECUTABLE)

$(OBJS): $(SRCS)
	$(CXX) $(CXXFLAGS) -c $(@:.o=.cpp)

clean:
	rm -f $(OBJS)
	rm -f $(EXECUTABLE)
	@echo All object files and executable removed
