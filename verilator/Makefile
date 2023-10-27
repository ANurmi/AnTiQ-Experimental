BUILD_DIR ?= $(realpath $(CURDIR))

.PHONY: compile
compile:
	cd $(BUILD_DIR)
	./scripts/verilate.sh

.PHONY: run
run:
	./obj_dir/Vpq

.PHONY: gui
gui:
	gtkwave waveform.vcd

.PHONY: clean
clean:
	rm -fr obj_dir
	rm waveform.vcd