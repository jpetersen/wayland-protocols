AC_PREREQ([2.64])

m4_define([wayland_protocols_major_version], [0])
m4_define([wayland_protocols_minor_version], [1])
m4_define([wayland_protocols_micro_version], [0])
m4_define([wayland_protocols_version],
          [wayland_protocols_major_version.wayland_protocols_minor_version.wayland_protocols_micro_version])

AC_INIT([wayland-protocols],
        [wayland_protocols_version],
        [https://bugs.freedesktop.org/enter_bug.cgi?product=Wayland&component=protocols&version=wayland-protocols_version],
        [wayland-protocols],
        [http://wayland.freedesktop.org/])

AC_SUBST([WAYLAND_PROTOCOLS_VERSION_MAJOR], [wayland_protocols_major_version])
AC_SUBST([WAYLAND_PROTOCOLS_VERSION_MINOR], [wayland_protocols_minor_version])
AC_SUBST([WAYLAND_PROTOCOLS_VERSION_MICRO], [wayland_protocols_micro_version])
AC_SUBST([WAYLAND_PROTOCOLS_VERSION], [wayland_protocols_version])

AM_INIT_AUTOMAKE([1.11 foreign no-dist-gzip dist-xz])

AM_SILENT_RULES([yes])

PKG_PROG_PKG_CONFIG()

AC_CONFIG_FILES([
	Makefile
	wayland-protocols.pc
	])
AC_OUTPUT

AC_MSG_RESULT([
	Prefix			${prefix}
	])
