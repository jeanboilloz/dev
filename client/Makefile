# PROJET client : Fichier Makefile
include ../../../Makefile.inc

PSE_DIR=../../..

CC = gcc

SRC=$(wildcard *.c)
OBJ=$(SRC:.c=.o)
EXE=client

all: $(SRC) $(EXE)

$(EXE): $(OBJ)
	$(CC) $(OBJ) -o $@ $(LDLIBS)
%.o: %.c defs.h
	$(CC) -c $(CFLAGS) $< -o $@

clean :
	rm -f *.o $(EXE)
