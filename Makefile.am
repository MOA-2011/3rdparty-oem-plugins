ACLOCAL_AMFLAGS = -I m4

SUBDIRS = \
        backupsuite \
		3gmodemmanager \
		hbbtv \
		ondemand \
		permanenttimeshift \
		shoutcast \
		autobouquetsmaker


metadir = $(datadir)/meta
#meta_DATA = index-enigma2-plugins.xml
#CLEANFILES = index-enigma2-plugins.xml

index-enigma2-plugins.xml: $(top_srcdir)/genmetaindex.py $(top_srcdir)/*/meta/plugin_*.xml
	$(AM_V_GEN)$(PYTHON) $^ > $@
