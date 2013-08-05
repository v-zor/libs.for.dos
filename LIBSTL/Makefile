CXX=gpp.exe
LD=ld.exe
AR=ar.exe
RANLIB=ranlib.exe
CFLAGS=-O
INCLUDES=
all: libstl 

libstl: dbfunctional.o dbstring.o dbvector.o
	$(AR) rcu libstl-dos.a *.o
	$(RANLIB) libstl-dos.a	

dbfunctional.o:
	$(CXX) $(INCLUDES) -c DBFUNCTIONAL.CPP
dbstring.o:
	$(CXX) $(INCLUDES) -c DBSTRING.CPP
dbvector.o:
	$(CXX) $(INCLUDES) -c DBVECTOR.CPP

clean:
	del *.o;
