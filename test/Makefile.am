
noinst_PROGRAMS =
EXTRA_DIST =

################################################################################
# lsudev
################################################################################

if WITH_UDEV

noinst_PROGRAMS += lsudev

lsudev_SOURCES  = lsudev.c
lsudev_CPPFLAGS = $(GUDEV_CFLAGS)
lsudev_LDADD    = $(GUDEV_LIBS)

endif

################################################################################
# mmtty
################################################################################

noinst_PROGRAMS += mmtty

mmtty_SOURCES = mmtty.c

mmtty_CPPFLAGS = \
	$(MM_CFLAGS) \
	-I$(top_srcdir) \
	-I$(top_srcdir)/src \
	-I$(top_srcdir)/src/kerneldevice \
	-I$(top_srcdir)/include \
	-I$(top_builddir)/include \
	-I$(top_srcdir)/libmm-glib \
	-I$(top_srcdir)/libmm-glib/generated \
	-I$(top_builddir)/libmm-glib/generated
	$(NULL)

mmtty_LDADD = \
	$(MM_LIBS) \
	$(top_builddir)/src/libport.la \
	$(NULL)

################################################################################
# mmrules
################################################################################

noinst_PROGRAMS += mmrules

mmrules_SOURCES = mmrules.c

mmrules_CPPFLAGS = \
	$(MM_CFLAGS) \
	-I$(top_srcdir) \
	-I$(top_srcdir)/src \
	-I$(top_srcdir)/src/kerneldevice \
	-I$(top_srcdir)/include \
	-I$(top_builddir)/include \
	-I$(top_srcdir)/libmm-glib \
	-I$(top_srcdir)/libmm-glib/generated \
	-I$(top_builddir)/libmm-glib/generated
	$(NULL)

mmrules_LDADD = \
	$(MM_LIBS) \
	$(top_builddir)/src/libkerneldevice.la \
	$(NULL)

################################################################################
# mmcli-test-sms
################################################################################

EXTRA_DIST += mmcli-test-sms
