#---------------------------------------------
# Macro declared in "DeclareMRPTLib.cmake":
#---------------------------------------------
define_mrpt_lib(
	# Lib name
	comms
	# Dependencies
	mrpt-base
	)

IF(CMAKE_MRPT_HAS_FTDI_SYSTEM)
	TARGET_LINK_LIBRARIES(mrpt-comms PRIVATE ${FTDI_LIBS})
ENDIF()
