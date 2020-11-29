bin_PROGRAMS = gde2-session-save gde2-session-inhibit

AM_CPPFLAGS =					\
	$(GDE2_SESSION_CFLAGS)			\
	$(DBUS_GLIB_CFLAGS)			\
	-DLOCALE_DIR=\""$(datadir)/locale"\"	\
	$(DISABLE_DEPRECATED_CFLAGS)

AM_CFLAGS = $(WARN_CFLAGS)

gde2_session_save_SOURCES =			\
	gde2-session-save.c

gde2_session_save_LDADD =			\
	$(SM_LIBS)				\
	$(ICE_LIBS)				\
	$(GDE2_SESSION_LIBS)			\
	$(DBUS_GLIB_LIBS)

gde2_session_inhibit_SOURCES =			\
	gde2-session-inhibit.c

gde2_session_inhibit_CPPFLAGS =			\
	$(AM_CPPFLAGS)				\
	$(GDE2_SESSION_CFLAGS)			\
	-DLOCALE_DIR=\""$(datadir)/locale"\"	\
	$(DISABLE_DEPRECATED_CFLAGS)

gde2_session_inhibit_LDADD =			\
	$(GDE2_SESSION_LIBS)

-include $(top_srcdir)/git.mk
