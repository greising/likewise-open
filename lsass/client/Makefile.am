compat_subdirs = \
    api \
    ad

full_subdirs = \
    $(compat_subdirs) \
    ntlm \
    rpc

lib_LTLIBRARIES = liblsaclient.la

liblsaclient_la_SOURCES =

liblsaclient_la_LIBADD = \
    @builddir@/api/liblsaclient_api.la \
    @builddir@/ad/liblsaclient_ad.la

if ENABLE_COMPAT
SUBDIRS=$(compat_subdirs)
else
SUBDIRS=$(full_subdirs)
endif

