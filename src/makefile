ifeq ($(shell uname -s), Darwin)
	CC = clang
else
	CC = gcc
	CFLAGS += -pthread -lm
endif

CFLAGS += -O2 -std=c99 

all: recwe.c recce.c
	${CC} recwe.c ${CFLAGS} -o recwe
	${CC} recce.c ${CFLAGS} -o recce
clean: 
	rm recwe recce
