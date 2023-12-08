ASM=sjasmplus
# -DZC for Z-Controller -DDIVMMC - for divMMC ports
FLAGS=-DZC 
SOURCES:=$(shell find bdos -type f -iname  "*.z80") $(shell find bios -type f -iname  "*.z80") cpm.z80
BLOBS:=$(shell find blob -type f -iname "*.bin")
PACKER=zx7b

cpm.\$c: page3.zx7 page7.zx7 loader.z80
		$(ASM) loader.z80

page3.zx7: page3.bin
		$(PACKER) page3.bin page3.zx7

page7.zx7: page7.bin
		$(PACKER) page7.bin page7.zx7

page3.bin page7.bin: $(SOURCES) $(BLOBS)
		$(ASM) $(FLAGS) cpm.z80

all: cpm.\$c

clean:
		rm -rf page*.bin page*.zx7 cpm.sna cpm.\$$c