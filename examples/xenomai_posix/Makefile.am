#------------------------------------------------------------------------------
#
#  $Id$
#
#  Copyright (C) 2006-2008  Florian Pose, Ingenieurgemeinschaft IgH
#
#  This file is part of the IgH EtherCAT Master.
#
#  The IgH EtherCAT Master is free software; you can redistribute it and/or
#  modify it under the terms of the GNU General Public License version 2, as
#  published by the Free Software Foundation.
#
#  The IgH EtherCAT Master is distributed in the hope that it will be useful,
#  but WITHOUT ANY WARRANTY; without even the implied warranty of
#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General
#  Public License for more details.
#
#  You should have received a copy of the GNU General Public License along with
#  the IgH EtherCAT Master; if not, write to the Free Software Foundation,
#  Inc., 51 Franklin St, Fifth Floor, Boston, MA  02110-1301  USA
#
#  ---
#  
#  The license mentioned above concerns the source code only. Using the
#  EtherCAT technology and brand is only permitted in compliance with the
#  industrial property and similar rights of Beckhoff Automation GmbH.
#
#------------------------------------------------------------------------------


AM_CFLAGS = -Wall

noinst_PROGRAMS = ec_xenomai_posix_example

ec_xenomai_posix_example_SOURCES = main.c
ec_xenomai_posix_example_CFLAGS = -I"$(XENOMAI_DIR)"/include -D_GNU_SOURCE -D_REENTRANT -Wall -pipe -D__XENO__ -I"$(XENOMAI_DIR)"/include/posix -I$(top_srcdir)/include
ec_xenomai_posix_example_LDFLAGS = -Wl,@"$(XENOMAI_DIR)"/lib/posix.wrappers -L"$(XENOMAI_DIR)"/lib -lpthread_rt -lrtdm -L$(top_builddir)/lib/.libs -lethercat -lrtdk -lxenomai -lpthread


#------------------------------------------------------------------------------
