# ======================================================================
#  FILE:  $URL$
# ======================================================================
#  PROJECT:             :  plex-motor_control_test
#  VERSION              :  @VERION@
#  LANGUAGE             :  CMake script
#  AUTHOR               :  @AUTHOR@
#  COPYRIGHT            :  @COPYRIGHT@
#  COMPILER             :  cmake version 3.0.2
#  CREATED              :  @CREATED@
#  CLASS                :  -
#  LAST MODIFIED        :  @LASTMODIFIED@
#  GENERATED FROM MODEL :  -
#  ORIGINAL MODEL AUTHOR:  -
# ----------------------------------------------------------------------
#  @DESCRIPTION@
# ----------------------------------------------------------------------
#  HISTORY
#  $History$
# ======================================================================

cmake_minimum_required(VERSION 3.2)

project(plex-motor_control_test)

include($ENV{ESROCOS_CMAKE})

#required function call to set up esrocos
esrocos_init()

########### FOR INTEGRATION PROJECTS ##############

#uncomment if you want to add dependencies for the build process (only required in integration projects)
esrocos_add_dependency(PARTITION x86_partition
                       MODULES   controldev)

########### FOR COMPONENT PROJECTS ################

#uncomment if you want to export a function
#esrocos_export_function("example" "tutorial/example_dir")

#uncomment to export PKG-CONFIG-file
#esrocos_export_pkgconfig( VERSION 1.0
#                          DESCRIPTION "none"
#                          REQUIRES ""
#                          LIBS ""
#                          STATIC_LIBS "" 
#                          C_FLAGS ""
#                        ) 
