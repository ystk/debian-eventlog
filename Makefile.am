
SUBDIRS = src tests solbuild 

EXTRA_DIST = VERSION NEWS PORTS CREDITS doc/API.txt doc/DESIGN.txt doc/configuration.txt \
	debian/changelog debian/changelog.in debian/compat debian/control debian/copyright \
	debian/libevtlog-dev.install debian/libevtlog0.install debian/libevtlog0.shlibs debian/rules \
	eventlog.spec.bb.in eventlog.spec.bb

pkgconfigdir = $(libdir)/pkgconfig
pkgconfig_DATA = eventlog.pc

debian/changelog: debian/changelog.in
	$(top_builddir)/config.status --file $@:$<
