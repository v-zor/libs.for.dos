CXX=gpp.exe
LD=ld.exe
AR=ar.exe
RANLIB=ranlib.exe
CFLAGS=-O
INCLUDES=-IC:\DJGPP\LIBSTL
all: libactor

libactor: actor.o actorevent.o actormailbox.o 
	$(AR) rcu libactor-dos.a *.o 
	$(RANLIB) libactor-dos.a	

actor.o:
	$(CXX) $(INCLUDES) -c ACTOR.CPP
actorevent.o:
	$(CXX) $(INCLUDES) -c ACTOREVENT.CPP
actormailbox.o:
	$(CXX) $(INCLUDES) -c ACTORMAILBOX.CPP

clean:
	del *.o;
