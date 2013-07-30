# Makefile
shell=/bin/sh
CC=cc
CFLAGS=-O
CPP=/lib/cpp

EXECS=circle circle32

all:${EXECS}

circle:circle.c
	${CC} ${CFLAGS} $? -o $@

circle32:circle32.c
	${CC} ${CFLAGS} $? -o $@

clean	:
		rm -rf ${EXECS} *.o

.PHONY	: clean all
