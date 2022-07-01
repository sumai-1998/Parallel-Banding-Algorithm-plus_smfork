# CMakeLists.txt for Project_Name project

project(project)

# required cmake version
cmake_minimum_required(VERSION 2.8)


add_subdirectory(pba)
set (EXTRA_LIBS ${EXTRA_LIBS} Project_Name_pba)


ADD_EXECUTABLE(project main.cpp)


target_link_libraries (project ${EXTRA_LIBS})

