FILE(GLOB_RECURSE ALL_LIB_CPP *.h)

ADD_LIBRARY(spatial
  ${ALL_LIB_CPP}
)

SET_TARGET_PROPERTIES(spatial PROPERTIES LINKER_LANGUAGE CXX)

TARGET_LINK_LIBRARIES(spatial
  ${DEPS}
)
