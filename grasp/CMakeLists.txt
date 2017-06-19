add_executable (grasp_driver main.cpp canAPI.cpp RockScissorsPaper.cpp)
target_link_libraries (grasp_driver BHand pcanbasic pthread hiredis)
#install (TARGETS grasp DESTINATION ${PROJECT_SOURCE_DIR}/bin)
install (TARGETS grasp_driver DESTINATION ${PROJECT_BINARY_DIR}/bin)
