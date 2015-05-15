cmake_minimum_required(VERSION 2.8.9)

project(Slicer-TrackerStabilizer)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://github.com/lchauvin/Slicer-TrackerStabilizer")
set(EXTENSION_CATEGORY "IGT")
set(EXTENSION_CONTRIBUTORS "Laurent Chauvin (BWH), Jayender Jagadeesan (BWH), Andras Lasso (Queen's University)")
set(EXTENSION_DESCRIPTION "Smooth Linear Transforms")
set(EXTENSION_ICONURL "https://raw.github.com/lchauvin/Slicer-TrackerStabilizer/master/Slicer-TrackerStabilizer.png")
set(EXTENSION_SCREENSHOTURLS "http://www.example.com/Slicer/Extensions/Slicer-TrackerStabilizer/Screenshots/1.png")

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(TrackerStabilizer)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_CPACK})
