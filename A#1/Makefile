# Make file
CC=gcc
CFLAG= -c -Wall

EXECS := circle
PROG = circle.c
OBJS := $(addprefix OBJECTS/, $(addsuffix .o, $(EXECS)))

all 	:$(EXECS)

OBJECTS	:
		mkdir -p $@

$(OBJS)	:| OBJECTS

$(EXECS):$(OBJS)
		$(CC) $^ -o $@

OBJECTS/circle.o	:$(PROG)
		$(CC) $(CFLAG) $^ -o $@

clean	:
		rm -rf $(EXECS) OBJECTS

.PHONY	: clean all
