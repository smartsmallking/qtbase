# Generated from qhostinfo.pro.

if(NOT QT_FEATURE_private_tests)
    return()
endif()

#####################################################################
## tst_qhostinfo Test:
#####################################################################

add_qt_test(tst_qhostinfo
    SOURCES
        tst_qhostinfo.cpp
    PUBLIC_LIBRARIES
        Qt::CorePrivate
        Qt::NetworkPrivate
)

#### Keys ignored in scope 1:.:.:qhostinfo.pro:<TRUE>:
# _REQUIREMENTS = "qtConfig(private_tests)"

## Scopes:
#####################################################################

extend_target(tst_qhostinfo CONDITION WIN32
    PUBLIC_LIBRARIES
        ws2_32
)
