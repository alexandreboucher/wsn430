WSN430 = ../../../..
FREERTOS = $(WSN430)/OS/FreeRTOS

SOURCE_PATH = $(FREERTOS)/Source
PORT_PATH = $(FREERTOS)/Source/portable/GCC/MSP430F449

NAMES = sink_example_cc1101


INCLUDES  = -I. -Imac -Iinterface
INCLUDES += -I$(WSN430)/drivers
INCLUDES += -I$(WSN430)/lib/phy/simplephy
INCLUDES += -I$(FREERTOS)/Source/include

SRC  = main.c
SRC += mac/mac.c
SRC += interface/interface.c

SRC += $(WSN430)/lib/phy/simplephy/simplephy.c
SRC += $(WSN430)/drivers/cc1101.c

SRC += $(SOURCE_PATH)/tasks.c
SRC += $(SOURCE_PATH)/list.c
SRC += $(SOURCE_PATH)/queue.c
SRC += $(SOURCE_PATH)/portable/MemMang/heap_1.c
SRC += $(PORT_PATH)/port.c
SRC += $(WSN430)/drivers/spi1.c
SRC += $(WSN430)/drivers/clock.c
SRC += $(WSN430)/drivers/timerB.c
SRC += $(WSN430)/drivers/ds2411.c
SRC += $(WSN430)/drivers/uart0.c

include $(WSN430)/drivers/Makefile.common

