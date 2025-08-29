project(CFE_HK C)
# This file is from https://github.com/cfs-apps/proxy_hk

include_directories(fsw/inc)
include_directories(fsw/src)

aux_source_directory(fsw/src APP_SRC_FILES)
aux_source_directory(fsw/tables APP_TABLE_FILES)

# Create the app module
add_cfe_app(hk ${APP_SRC_FILES})
add_cfe_tables(hk ${APP_TABLE_FILES})

