#
# Makefile.am
#

AM_CFLAGS=-I$(top_srcdir)/include -I$(top_srcdir)/include/dicom
AM_CXXFLAGS=-I$(top_srcdir)/include -I$(top_srcdir)/include/dicom

bin_PROGRAMS = label_area
label_area_SOURCES=label_area.c
label_area_LDADD= $(addprefix $(top_builddir)/, $(LIBS_MGH))
label_area_LDFLAGS=$(OS_LDFLAGS)

# Our release target. Include files to be excluded here. They will be
# found and removed after 'make install' is run during the 'make
# release' target.
EXCLUDE_FILES=""
include $(top_srcdir)/Makefile.extra
