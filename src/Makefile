ifeq ($(DEBUG),1)
DBGFLAGS=-d2 -od -hd
else
DBGFLAGS=-d0 -ox -ot
endif

%.exe: %.c
	wcl386 $(DBGFLAGS) -we -za99 -bc -fp6 -sg -k1m -l=OS2V2 -fe=$@ $<

.PHONY: all
all: # default target

all: mptable.exe
