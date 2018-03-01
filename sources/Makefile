
its-y += snickerdoodle.ub
its-y += snickerdoodle-black.ub
its-y += snickerdoodle-prime.ub

all : $(its-y) dts/

%.ub : %.its
	@mkimage -A arm -n "snickerdoodle Linux FIT image" -f $< $@

clean :
	@rm -f $(its-y)


