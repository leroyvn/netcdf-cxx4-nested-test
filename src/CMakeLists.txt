find_package(NetCDF REQUIRED)

add_executable(main main.cpp)
target_include_directories(main 
        PRIVATE 
            ${NCXX_INCLUDE_DIRS}
            ${NetCDF_INCLUDE_DIRS}
)
target_link_libraries(main PRIVATE netcdf-cxx4)
target_compile_features(main PRIVATE cxx_std_11)