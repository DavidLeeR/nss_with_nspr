OBJ = jar-ds.o jar.o jarfile.o jarint.o jarsign.o jarver.o 
CC = gcc

libjar.a: $(OBJ)
	ar rcs libjar.a $(OBJ)

jar-ds.o: jar-ds.c
	$(CC) -c jar-ds.c

jar.o: jar.c
	$(CC) -c jar.c

jarfile.o: jarfile.c
	$(CC) -c jarfile.c

jarint.o: jarint.c
	$(CC) -c jarint.c

jarsign.o: jarsign.c
	$(CC) -c jarsign.c

jarver.o: jarver.c
	$(CC) -c jarver.c

clean:
	rm *.o

