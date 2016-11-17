themedir = $(datadir)/plymouth/themes/milislinux
nodist_theme_DATA = \
                    milislinux.plymouth

dist_theme_DATA =                                                     \
                    milislinux.script                                  \
                    logo_blurred.png                              \
                    logo.png


MAINTAINERCLEANFILES = Makefile.in milislinux.plymouth
CLEANFILES = milislinux.plymouth

milislinux.plymouth: $(srcdir)/milislinux.plymouth.in
	sed -e 's,[@]PLYMOUTH_THEME_PATH[@],$(PLYMOUTH_THEME_PATH),g' \
	       $(srcdir)/milislinux.plymouth.in > milislinux.plymouth

EXTRA_DIST = milislinux.plymouth.in
