SIM ?= icarus
TOPLEVEL_LANG ?= verilog
VERILOG_SOURCES += $(PWD)/../hdl/dut.v
VERILOG_SOURCES += $(PWD)/wrappers/xor_test.v
TOPLEVEL = xor_test
MODULE = dut_test

or:
	rm -rf sim_build
	$(MAKE) sim MODULE=$(MODULE) TOPLEVEL=$(TOPLEVEL)
include $(shell cocotb-config --makefiles)/Makefile.sim
