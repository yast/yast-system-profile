# Makefile.am for system-profile/src

yncludedir = @yncludedir@/system-profile

client_DATA =			\
	system-profile.ycp		\
	system-profile_auto.ycp

ynclude_DATA =			\
	texts.ycp		\
	dialogs.ycp	

desktop_DATA =			\
	system-profile.desktop

module_DATA =			\
	SystemProfile.ycp

rncdir = $(schemadir)/autoyast/rnc
rnc_DATA =			\
	 system-profile.rnc

# create a symlink for local build, #145327
system-profile:
	ln -sf . $@
ycpchook = system-profile

EXTRA_DIST = $(client_DATA) $(ynclude_DATA) $(module_DATA) $(desktop_DATA) $(rnc_DATA)

include $(top_srcdir)/Makefile.am.common
