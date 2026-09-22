# This file is part of Hercules.
set(HERC_PLUGIN_NAME ExtendedBG_char)

# eBG_common.c is #include'd directly by ExtendedBG-char.c -- only list the driver file.
set(HERC_PLUGIN_C
  ExtendedBG-char.c
)
set(HERC_PLUGIN_H
  eBG_common.h
)

add_plugin_target(${HERC_PLUGIN_NAME}
  CFILES
    ${HERC_PLUGIN_C}
    ${HERC_PLUGIN_H}
)
