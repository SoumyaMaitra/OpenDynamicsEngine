# Makefile Mac
TOP_SRCDIR = ~/Users/shomu/Downloads/ODE-DrGuero/ODE/ode-0.16.4
NAME=biped
CC=gcc
CXX=g++
# Mac specific flags (brew install ode)
CXXFLAGS=-mmacosx-version-min=10.13 -arch arm64 -lode

# Mac
LIBS = -L/usr/local/lib -lode -ldrawstuff -lpthread -framework GLUT -framework OpenGL -lm
LIBDIR = -L/usr/local/lib -lode -ldrawstuff -lpthread -framework GLUT -framework OpenGL -lm
INCDIR = -I$(TOP_SRCDIR)/include -I$(TOP_SRCDIR)/ode/src -I/usr/include -I/usr/include/GL

OBJS = biped.cpp core.cpp
all: 
	$(CXX) -o ${NAME} ${OBJS} $(INCDIR) $(LIBDIR) $(LIB)	

clean:
	rm  $(OBJS)  *~  *.*~

.PHONY: all clean