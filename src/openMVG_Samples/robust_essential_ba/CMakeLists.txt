
ADD_DEFINITIONS(-DTHIS_SOURCE_DIR="${CMAKE_CURRENT_SOURCE_DIR}")

ADD_EXECUTABLE(openMVG_sample_robustEssential_ba robust_essential_ba.cpp)
TARGET_LINK_LIBRARIES(openMVG_sample_robustEssential_ba 
  openMVG_image
  openMVG_multiview
  vlsift
  stlplus
  flann_cpp_s
  ceres
  ${OPENMVG_LIBRARY_DEPENDENCIES})

