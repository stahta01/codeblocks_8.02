SUBDIRS = resources

INCLUDES = $(WX_CXXFLAGS) \
		-I$(top_srcdir)/src/include \
		-I$(top_srcdir)/src/include/wxscintilla/include

libdir = $(pkgdatadir)/plugins

lib_LTLIBRARIES = libprojectsimporter.la

libprojectsimporter_la_LDFLAGS = -module -version-info 0:1:0 -shared -no-undefined -avoid-version

libprojectsimporter_la_LIBADD = $(PLUGIN_WX_LIBS) ../../sdk/libcodeblocks.la

libprojectsimporter_la_SOURCES = projectsimporter.cpp \
				devcpploader.cpp \
				msvc7loader.cpp \
				msvc7workspaceloader.cpp \
				msvcloader.cpp \
				msvcworkspacebase.cpp \
				msvcworkspaceloader.cpp

noinst_HEADERS = projectsimporter.h \
				devcpploader.h \
				msvc7loader.h \
				msvc7workspaceloader.h \
				msvcloader.h \
				msvcworkspacebase.h \
				msvcworkspaceloader.h
