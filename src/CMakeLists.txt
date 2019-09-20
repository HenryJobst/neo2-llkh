include_directories(${CMAKE_SOURCE_DIR}/src)
 
set(MySources main.c trayicon.c)
set(Resources resources.rc)
set(Icons appicon.ico appicon-disabled.ico)

add_executable(neo2-llhk ${MySources} ${Resources} ${Icons})
 
target_link_libraries(neo2-llhk)
 
install(TARGETS neo2-llhk DESTINATION bin)
#install(TARGETS settings.ini DESTINATION bin)
