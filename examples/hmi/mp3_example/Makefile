#
# This is a project Makefile. It is assumed the directory this Makefile resides in is a
# project subdirectory.
#

PROJECT_NAME := lvgl_mp3
#If IOT_SOLUTION_PATH is not defined, use relative path as default value
IOT_SOLUTION_PATH ?= $(abspath $(shell pwd)/../../)

#add ADF_PATH
ADF_VER := $(shell cd ${ADF_PATH} && git describe --always --tags --dirty)
EXTRA_COMPONENT_DIRS += $(ADF_PATH)/components/
CPPFLAGS := -D ADF_VER=\"$(ADF_VER)\"

include $(IOT_SOLUTION_PATH)/Makefile
include $(IDF_PATH)/make/project.mk