CC = gcc
LDIR = ../../../dist/Debug/lib
LIBS = -L $(LDIR) -l freebl3 \
-L $(LDIR) -l mozpkix \
-L $(LDIR) -l nspr4 \
-L $(LDIR) -l nss3 \
-L $(LDIR) -l mozpkix-testlib \
-L $(LDIR) -l nssckbi \
-L $(LDIR) -l nssdbm3 \
-L $(LDIR) -l nssutil3 \
-L $(LDIR) -l plc4 \
-L $(LDIR) -l plds4 \
-L $(LDIR) -l sectool \
-L $(LDIR) -l smime3 \
-L $(LDIR) -l softokn3 \
-L $(LDIR) -l ssl3 \
-L $(LDIR) -l nss_zlib

signtool: certgen.o javascript.o list.o sign.o signtool.o util.o verify.o zip.o 
	$(CC) -o signtool certgen.o javascript.o list.o sign.o signtool.o util.o verify.o zip.o $(LIBS) -I.

certgen.o: certgen.c 
	$(CC) -c certgen.c

javascript.o: javascript.c
	$(CC) -c javascript.c

list.o: list.c
	$(CC) -c list.c

sign.o: sign.c
	$(CC) -c sign.c

signtool.o: signtool.c
	$(CC) -c signtool.c

util.o: util.c
	$(CC) -c util.c

verify.o: verify.c
	$(CC) -c verify.c

zip.o: zip.c
	$(CC) -c zip.c

clean: 
	rm *.o