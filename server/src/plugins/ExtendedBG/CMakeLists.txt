# This file is part of Hercules.
set(HERC_PLUGIN_NAME ExtendedBG)

# eBG_common.c and eBG_functions.c are #include'd directly by ExtendedBG.c
# (textual inclusion, not separate translation units) -- only list the driver file.
set(HERC_PLUGIN_C
  ExtendedBG.c
)
set(HERC_PLUGIN_H
  eBG_common.h
)

add_plugin_target(${HERC_PLUGIN_NAME}
  CFILES
    ${HERC_PLUGIN_C}
    ${HERC_PLUGIN_H}
)
