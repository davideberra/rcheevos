add_library(rcheevos
src/rc_version.c
src/rcheevos/value.c
src/rcheevos/operand.c
src/rcheevos/runtime_progress.c
src/rcheevos/alloc.c
src/rcheevos/rc_validate.c
src/rcheevos/rc_validate.h
src/rcheevos/lboard.c
src/rcheevos/consoleinfo.c
src/rcheevos/condset.c
src/rcheevos/condition.c
src/rcheevos/runtime.c
src/rcheevos/richpresence.c
src/rcheevos/format.c
src/rcheevos/memref.c
src/rcheevos/trigger.c
src/rcheevos/rc_internal.h
src/rc_compat.h
src/rc_client_external_versions.h
src/rc_client_internal.h
src/rc_client_raintegration.c
src/rc_client_raintegration_internal.h
src/rc_compat.c
src/rc_version.h
src/rc_util.c
src/rapi/rc_api_editor.c
src/rapi/rc_api_common.h
src/rapi/rc_api_runtime.c
src/rapi/rc_api_info.c
src/rapi/rc_api_user.c
src/rapi/rc_api_common.c
src/rhash/hash_rom.c
src/rhash/hash_disc.c
src/rhash/aes.c
src/rhash/cdreader.c
src/rhash/hash_zip.c
src/rhash/aes.h
src/rhash/md5.h
src/rhash/md5.c
src/rhash/hash.c
src/rhash/rc_hash_internal.h
src/rhash/hash_encrypted.c
include/rcheevos.h
include/rc_util.h
include/rc_api_info.h
include/rc_runtime_types.h
include/rc_api_runtime.h
include/rc_hash.h
include/rc_error.h
include/rc_client_raintegration.h
include/rc_api_request.h
include/rc_client.h
include/rc_runtime.h
include/rc_consoles.h
include/rc_api_user.h
include/rc_export.h
include/rc_api_editor.h
)

target_include_directories(rcheevos PRIVATE "${CMAKE_CURRENT_SOURCE_DIR}/include")
target_include_directories(rcheevos INTERFACE "${CMAKE_CURRENT_SOURCE_DIR}/include")
target_include_directories(rcheevos PRIVATE "${CMAKE_CURRENT_SOURCE_DIR}/src")
target_include_directories(rcheevos INTERFACE "${CMAKE_CURRENT_SOURCE_DIR}/src")
target_compile_definitions(rcheevos PRIVATE "RC_DISABLE_LUA=1")
