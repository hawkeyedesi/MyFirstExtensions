cmake_minimum_required(VERSION 2.8.9)

project(MyFirstExtensions)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://github.com/hawkeyedesi/MyFirstExtensions")
set(EXTENSION_CATEGORY "Learning")
set(EXTENSION_CONTRIBUTORS "Kashyap (The University of Iowa)")
set(EXTENSION_DESCRIPTION "This is an example in developer as part of the tutorial.")
set(EXTENSION_ICONURL "https://raw.github.com/hawkeyedesi/MyFirstExtensions/master/MyFirstExtensions.png")
set(EXTENSION_SCREENSHOTURLS "http://www.example.com/Slicer/Extensions/MyFirstExtensions/Screenshots/1.png")

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(LineIntensityProfile)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_CPACK})
