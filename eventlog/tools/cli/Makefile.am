bin_PROGRAMS = lw-eventlog-cli

lw_eventlog_cli_CPPFLAGS = \
	-I$(top_srcdir)/include \
	$(LWADVAPI_INCLUDES) \
	$(POPT_INCLUDES) \
	$(LIBXML2_INCLUDES)

lw_eventlog_cli_SOURCES = \
    evtparser.c \
    xmllookup.c \
    main.c


lw_eventlog_cli_LDADD = \
	$(top_builddir)/client/libeventlog.la \
	$(top_builddir)/utils/libeventlogutils.la \
	-llwadvapi \
	-llwadvapi_nothr \
	-lpopt \
	-lxml2

lw_eventlog_cli_LDFLAGS = \
	$(LWADVAPI_LDFLAGS) \
	$(POPT_LDFLAGS) \
	$(LIBXML2_LDFLAGS)
