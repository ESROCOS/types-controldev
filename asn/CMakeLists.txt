# H2020 ESROCOS Project
# Company: DFKI
# Licence: GPLv2

#esrocos_asn1_types_package(esrocos_types_controldev
#	controldev.asn
#        )
#
#esrocos_asn1_types_build_test(esrocos_types_controldev)
#esrocos_asn1_types_install(esrocos_types_controldev ${CMAKE_INSTALL_PREFIX}/types/controldev)

set (ASN_FILES controldev.asn)
configure_file (${PROJECT_NAME}.pc.in ${PROJECT_NAME}.pc @ONLY)
install (FILES ${CMAKE_CURRENT_BINARY_DIR}/${PROJECT_NAME}.pc DESTINATION ${CMAKE_INSTALL_PREFIX}/lib/pkgconfig)
install (FILES ${ASN_FILES} DESTINATION ${CMAKE_INSTALL_PREFIX}/types/controldev)
