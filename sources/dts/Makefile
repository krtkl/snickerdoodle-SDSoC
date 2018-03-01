#
# SPDX-License-Identifier:	GPL-2.0+
#


dtb-y += snickerdoodle.dtb
dtb-y += snickerdoodle-black.dtb
dtb-y += snickerdoodle-prime.dtb

all : $(dtb-y)

%.dtb : %.dts
	@echo "  $< --> $@"
	@dtc -@ -I dts -O dtb -o $@ $<

export DTSI_DIR=${PWD}

.PHONY : board_dtb

clean :
	@rm -f $(dtb-y)
