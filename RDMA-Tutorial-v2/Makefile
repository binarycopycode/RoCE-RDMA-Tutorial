CC=gcc
CFLAGS=-Wall
INCLUDES=
LDFLAGS=
LIBS= -lrdmacm -libverbs -lpthread

SRCS=main.c client.c config.c ib.c server.c setup_ib.c sock.c
OBJS=$(SRCS:.c=.o)
PROG=rdma-tutorial

all: $(PROG)

debug: CFLAGS=-Wall -g -DDEBUG
debug: $(PROG)

.c.o:
	$(CC) $(CFLAGS) $(INCLUDES) -c -o $@ $<

$(PROG): $(OBJS)
	$(CC) $(CFLAGS) $(INCLUDES) -o $@ $(OBJS) $(LDFLAGS) $(LIBS)

clean:
	$(RM) *.o *~ $(PROG)
