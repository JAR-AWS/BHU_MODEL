PRECISION  = DOUBLE
PROFILE    = FALSE

DEBUG      = FALSE

DIM        = 1
#DIM        = 2
#DIM        = 3

COMP	   = gnu

USE_MPI    = TRUE
#USE_OMP	   = TRUE

USE_GRAV   = TRUE

USE_MHD = FALSE


# define the location of the CASTRO top directory
CASTRO_HOME1 ?= $(CASTRO_HOME)

# This sets the EOS directory in $(MICROPHYSICS_HOME)/EOS
EOS_DIR     := gamma_law

# This sets the EOS directory in $(MICROPHYSICS_HOME)/Networks
NETWORK_DIR := general_null
NETWORK_INPUTS = ignition.net

PROBLEM_DIR ?= ./

Bpack	:= $(PROBLEM_DIR)/Make.package
Blocs	:= $(PROBLEM_DIR)

include $(CASTRO_HOME)/Exec/Make.Castro
