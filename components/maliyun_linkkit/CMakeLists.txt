
set(COMPONENT_ADD_INCLUDEDIRS "include")
set(COMPONENT_PRIV_INCLUDEDIRS ".")

set(COMPONENT_SRCS "maliyun_linkkit_gateway.c"
                    "maliyun_linkkit_list.c"
                    "maliyun_linkkit_platform.c"
                    "maliyun_linkkit_subdevice.c")

# requirements can't depend on config
set(COMPONENT_REQUIRES esp-aliyun mcommon mwifi mlink mupgrade json)

register_component()
