m4_define([accountsservice_version], [0.6.40])
m4_define([upower_required_version], [0.99.0])
m4_define([bt_required_version], [3.16.0])

PKG_CHECK_MODULES(STATUS_PLUGIN,
    [
     accountsservice >= accountsservice_version,
     upower-glib >= upower_required_version,
     gnome-bluetooth-1.0 >= bt_required_version
    ],
    [have_status=yes], [have_status=no]
)
AM_CONDITIONAL(ENABLE_STATUS_PLUGIN, test x$have_status = xyes)
AC_CONFIG_FILES([panel/applets/status/Makefile])
