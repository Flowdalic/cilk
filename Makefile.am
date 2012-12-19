SUBDIRS = cilk2c runtime support examples doc FAQ
EXTRA_DIST = THANKS bootstrap.sh
ACLOCAL_AMFLAGS = -I m4

all-check:
	$(MAKE) clean
	$(MAKE) check
	$(MAKE) clean
	$(MAKE) check CILKCFLAGS='-O2 -cilk-debug'
	$(MAKE) clean
	$(MAKE) check CILKCFLAGS='-O2 -cilk-profile'
	$(MAKE) clean
	$(MAKE) check CILKCFLAGS='-O2 -cilk-profile -cilk-debug'


