file(GLOB SRCS *.cpp)

ADD_EXECUTABLE(testSampleLib2 ${SRCS})

TARGET_LINK_LIBRARIES(
    testSampleLib2
    SAMPLE_LIB_2
    ${GTEST_LIBRARY}
    ${GMOCK_LIBRARY}
)

add_test(NAME testSampleLib2
         COMMAND testSampleLib2)
