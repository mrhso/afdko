# Copyright 2014 Adobe Systems Incorporated (http://www.adobe.com/). All Rights Reserved.
# This software is licensed as OpenSource, under the Apache License, Version 2.0. 
# This license is available at: http://opensource.org/licenses/Apache-2.0.

# Configuration
CONFIG = debug
CFLAGS = $(STD_OPTS) -g -DCFF_T13_SUPPORT=1 -DCFFREAD_DEBUG=1

# Library
SRC_DIR = $(ROOT_DIR)/source/cffread
LIB_SRCS = $(SRC_DIR)/cffread.c
LIB_OBJS = cffread.o
LIB_TARGET = $(LIB_DIR)/cffread.a

# Build targets
TARGETS = $(LIB_TARGET)

# Standard definitions
include ../../../standard/linux.mak

# Auto-generated dependencies
include depend.mak

# Object rules
cffread.o:
	$(CC) $(CFLAGS) -c $(SRC_DIR)/cffread.c -o $@
