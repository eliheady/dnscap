MAINTAINERCLEANFILES = $(srcdir)/Makefile.in

AM_CFLAGS = -I$(srcdir) \
    -I$(top_srcdir)/src \
    -I$(top_srcdir)/isc \
    $(SECCOMPFLAGS)

if HAVE_LDNS
pkglib_LTLIBRARIES = rzkeychange.la
rzkeychange_la_SOURCES = rzkeychange.c hashtbl.c
dist_rzkeychange_la_SOURCES = hashtbl.h
rzkeychange_la_LDFLAGS = -module -avoid-version $(LIBRARY_VERSION)
endif
