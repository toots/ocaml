BASEDIR=../..
LIBRARIES=unix
ADD_COMPFLAGS=-I $(OTOPDIR)/otherlibs/$(UNIXLIBVAR)unix
LD_PATH=$(TOPDIR)/otherlibs/$(UNIXLIBVAR)unix

default: reflector.exe fdstatus.exe
	@$(SET_LD_PATH) $(MAKE) run-all

include $(BASEDIR)/makefiles/Makefile.several
include $(BASEDIR)/makefiles/Makefile.common

%.exe: %.c
	@$(BYTECC) -o $*.exe $*.c > /dev/null
