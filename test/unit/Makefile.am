# -*- Makefile -*-
#
# Copyright 2011 Sandia Corporation. Under the terms of Contract
# DE-AC04-94AL85000 with Sandia Corporation, the U.S.  Government
# retains certain rights in this software.
# 
# This file is part of the Portals SHMEM software package. For license
# information, see the LICENSE file in the top level directory of the
# distribution.
#

all: $(check_PROGRAMS)

check_PROGRAMS = $(TESTS)

TESTS = \
	hello \
	circular_shift \
	accessible_ping \
	max_reduction \
	big_reduction \
	to_all \
	strided_put \
	barrier \
	bcast \
	put1 \
	get1 \
	swap1 \
	ping \
	pingpong \
	shmalloc \
	shrealloc \
	shmemalign \
	get_g \
	iput32 \
	iput64 \
	iput128 \
	iput_short \
	iput_double \
	iput_float \
	iput_long \
	iput_longdouble \
	iput_longlong \
	sping \
	pingpong-short \
	ipgm \
	iput-iget \
	swapm \
	cswap \
	waituntil \
	atomic_inc \
	set_lock \
	test_lock \
	fcollect64 \
	bigput \
	bigget \
	ns \
	bcast_flood \
	lfinc

if HAVE_FORTRAN
TESTS += \
     hello_f
endif

PROCS ?= 2

TESTS_ENVIRONMENT = yod -np $(PROCS)

AM_CPPFLAGS = -I$(top_srcdir)/mpp
AM_FCFLAGS = -I$(top_srcdir)/mpp
AM_LDFLAGS = $(LIBTOOL_WRAPPER_LDFLAGS)

hello_SOURCES = hello.c
hello_LDADD = $(top_builddir)/src/libsma.la

hello_f_SOURCES = hello_f.f90
hello_f_LDADD = $(top_builddir)/src/libsma.la

circular_shift_SOURCES = circular_shift.c
circular_shift_LDADD = $(top_builddir)/src/libsma.la

accessible_ping_SOURCES = accessible_ping.c
accessible_ping_LDADD = $(top_builddir)/src/libsma.la

max_reduction_SOURCES = max_reduction.c
max_reduction_LDADD = $(top_builddir)/src/libsma.la

big_reduction_SOURCES = big_reduction.c
big_reduction_LDADD = $(top_builddir)/src/libsma.la

strided_put_SOURCES = strided_put.c
strided_put_LDADD = $(top_builddir)/src/libsma.la

barrier_SOURCES = barrier.c
barrier_LDADD = $(top_builddir)/src/libsma.la

bcast_SOURCES = bcast.c
bcast_LDADD = $(top_builddir)/src/libsma.la

put1_SOURCES = put1.c
put1_LDADD = $(top_builddir)/src/libsma.la

get1_SOURCES = get1.c
get1_LDADD = $(top_builddir)/src/libsma.la

swap1_SOURCES = swap1.c
swap1_LDADD = $(top_builddir)/src/libsma.la

ping_SOURCES = ping.c
ping_LDADD = $(top_builddir)/src/libsma.la

pingpong_SOURCES = pingpong.c
pingpong_LDADD = $(top_builddir)/src/libsma.la

iput32_SOURCES = iput32.c
iput32_LDADD = $(top_builddir)/src/libsma.la

iput64_SOURCES = iput64.c
iput64_LDADD = $(top_builddir)/src/libsma.la

iput128_SOURCES = iput128.c
iput128_LDADD = $(top_builddir)/src/libsma.la

iput_short_SOURCES = iput_short.c
iput_short_LDADD = $(top_builddir)/src/libsma.la

iput_double_SOURCES = iput_double.c
iput_double_LDADD = $(top_builddir)/src/libsma.la

iput_float_SOURCES = iput_float.c
iput_float_LDADD = $(top_builddir)/src/libsma.la

iput_long_SOURCES = iput_long.c
iput_long_LDADD = $(top_builddir)/src/libsma.la

iput_longdouble_SOURCES = iput_longdouble.c
iput_longdouble_LDADD = $(top_builddir)/src/libsma.la

iput_longlong_SOURCES = iput_longlong.c
iput_longlong_LDADD = $(top_builddir)/src/libsma.la

sping_SOURCES = sping.c
sping_LDADD = $(top_builddir)/src/libsma.la

pingpong_short_SOURCES = pingpong-short.c
pingpong_short_LDADD = $(top_builddir)/src/libsma.la

iput_iget_SOURCES = iput-iget.c
iput_iget_LDADD = $(top_builddir)/src/libsma.la

ipgm_SOURCES = ipgm.c
ipgm_LDADD = $(top_builddir)/src/libsma.la

shmalloc_SOURCES = shmalloc.c
shmalloc_LDADD = $(top_builddir)/src/libsma.la

shrealloc_SOURCES = shrealloc.c
shrealloc_LDADD = $(top_builddir)/src/libsma.la

shmemalign_SOURCES = shmemalign.c
shmemalign_LDADD = $(top_builddir)/src/libsma.la

get_g_SOURCES = get_g.c
get_g_LDADD = $(top_builddir)/src/libsma.la

swapm_SOURCES = swapm.c
swapm_LDADD = $(top_builddir)/src/libsma.la

cswap_SOURCES = cswap.c
cswap_LDADD = $(top_builddir)/src/libsma.la

waituntil_SOURCES = waituntil.c
waituntil_LDADD = $(top_builddir)/src/libsma.la

atomic_inc_SOURCES = atomic_inc.c
atomic_inc_LDADD = $(top_builddir)/src/libsma.la

set_lock_SOURCES = set_lock.c
set_lock_LDADD = $(top_builddir)/src/libsma.la

test_lock_SOURCES = test_lock.c
test_lock_LDADD = $(top_builddir)/src/libsma.la

fcollect64_SOURCES = fcollect64.c
fcollect64_LDADD = $(top_builddir)/src/libsma.la

bigput_SOURCES = bigput.c
bigput_LDADD = $(top_builddir)/src/libsma.la

bigget_SOURCES = bigget.c
bigget_LDADD = $(top_builddir)/src/libsma.la

to_all_SOURCES = to_all.c
to_all_LDADD = $(top_builddir)/src/libsma.la

ns_SOURCES = ns.c
ns_LDADD = $(top_builddir)/src/libsma.la

bcast_flood_SOURCES = bcast_flood.c
bcast_flood_LDADD = $(top_builddir)/src/libsma.la

lfinc_SOURCES = lfinc.c
lfinc_LDADD = $(top_builddir)/src/libsma.la