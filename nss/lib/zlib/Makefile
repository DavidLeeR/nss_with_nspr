OBJ = adler32.o compress.o crc32.o deflate.o gzclose.o gzlib.o gzread.o gzwrite.o infback.o inffast.o inflate.o inftrees.o trees.o uncompr.o zutil.o
CC = gcc

libnss_zlib.a: $(OBJ)
	ar rcs libnss_zlib.a $(OBJ)

adler32.o: adler32.c
	$(CC) -c adler32.c

compress.o: compress.c
	$(CC) -c compress.c

crc32.o: crc32.c
	$(CC) -c crc32.c

deflate.o: deflate.c
	$(CC) -c deflate.c

gzclose.o: gzclose.c
	$(CC) -c gzclose.c

gzlib.o: gzlib.c
	$(CC) -c gzlib.c

gzread.o: gzread.c
	$(CC) -c gzread.c

gzwrite.o: gzwrite.c
	$(CC) -c gzwrite.c

infback.o: infback.c
	$(CC) -c infback.c

inffast.o: inffast.c
	$(CC) -c inffast.c

inflate.o: inflate.c
	$(CC) -c inflate.c

inftrees.o: inftrees.c
	$(CC) -c inftrees.c

trees.o: trees.c
	$(CC) -c trees.c

uncompr.o: uncompr.c
	$(CC) -c uncompr.c

zutil.o: zutil.c
	$(CC) -c zutil.c

clean:
	rm *.o