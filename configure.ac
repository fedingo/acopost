#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ([2.68])
AC_INIT([acopost], [1.8.7], [ulrikp@users.sourceforge.net])
AM_INIT_AUTOMAKE([-Wall])
AC_CONFIG_SRCDIR([src/t3.c])
AC_CONFIG_HEADERS([config.h])

# Checks for programs.
AC_PROG_CC
# AC_PROG_LEX

# Checks for libraries.
AC_CHECK_LIB([m], [log])

# Checks for header files.
AC_CHECK_HEADERS([limits.h stddef.h stdint.h stdlib.h string.h strings.h sys/time.h unistd.h values.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_TYPE_SIZE_T
AC_CHECK_TYPES([ptrdiff_t])

# Checks for library functions.
AC_FUNC_ERROR_AT_LINE
AC_FUNC_MALLOC
AC_FUNC_REALLOC
AC_CHECK_FUNCS([floor memmove memset sqrt strchr strcspn strdup strerror strpbrk strrchr strspn strstr])

AC_CONFIG_FILES([doc/Makefile
                 doc/ug/Makefile
                 language-models/Makefile
                 language-models/t3/Makefile
                 bin/Makefile
                 src/Makefile
                 Makefile
                 acopost.spec])
AC_OUTPUT