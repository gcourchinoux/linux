KBUILD_DEFCONFIG := gaspard_defconfig

KBUILD_CFLAGS += -pipe -D__linux__ -G 0 -msoft-float
KBUILD_AFLAGS += $(KBUILD_CFLAGS)

head-y := arch/gaspard/kernel/head.o

core-y += arch/gaspard/kernel/
core-y += arch/gaspard/mm/
LIBGCC := $(shell $(CC) $(KBUILD_CFLAGS) -print-libgcc-file-name)
libs-y += $(LIBGCC)
libs-y += arch/gaspard/lib/

drivers-y += arch/gaspard/drivers/
