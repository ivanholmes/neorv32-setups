# neorv32-setups: Exemplary FPGA Board Setups

[![Containers](https://img.shields.io/github/workflow/status/stnolting/neorv32-setups/Containers/main?longCache=true&style=flat-square&label=Containers&logo=Github%20Actions&logoColor=fff)](https://github.com/stnolting/neorv32-setups/actions?query=workflow%3AContainers)
[![Implementation](https://img.shields.io/github/workflow/status/stnolting/neorv32-setups/Implementation/main?longCache=true&style=flat-square&label=Implementation&logo=Github%20Actions&logoColor=fff)](https://github.com/stnolting/neorv32-setups/actions?query=workflow%3AImplementation)
[![Gitter](https://img.shields.io/badge/Chat-on%20gitter-4db797.svg?longCache=true&style=flat-square&logo=gitter&logoColor=e8ecef)](https://gitter.im/neorv32/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)


This folder provides exemplary [**NEORV32**](https://github.com/stnolting/neorv32) SoC setups and projects for different FPGA platforms/boards.
You can directly use one of the provided setups or use them as starting point to build your own setup.
Project maintainers may make pull requests against this repository to [add or link their setups](#Adding-Your-Project-Setup).


## Setups using Commercial Toolchains

| Setup | Toolchain | Board | FPGA | Author(s) |
|:------|:----------|:------|:-----|:----------|
| :file_folder: [`de0-nano-test-setup`](https://github.com/stnolting/neorv32-setups/tree/main/quartus/de0-nano-test-setup) | Intel Quartus Prime | [Terasic DE0-Nano](https://www.terasic.com.tw/cgi-bin/page/archive.pl?Language=English&CategoryNo=139&No=593)                     | Intel Cyclone IV `EP4CE22F17C6N`          | [stnolting](https://github.com/stnolting) |
| :file_folder: [`de0-nano-test-setup-qsys`](quartus/de0-nano-test-setup-qsys) | Intel Quartus Prime | [Terasic DE0-Nano](https://www.terasic.com.tw/cgi-bin/page/archive.pl?Language=English&CategoryNo=139&No=593)                     | Intel Cyclone IV `EP4CE22F17C6N`          | [torerams](https://github.com/torerams) |
| :file_folder: [`de0-nano-test-setup-avalonmm`](quartus/de0-nano-test-setup-avalonmm-wrapper) | Intel Quartus Prime | [Terasic DE0-Nano](https://www.terasic.com.tw/cgi-bin/page/archive.pl?Language=English&CategoryNo=139&No=593)                     | Intel Cyclone IV `EP4CE22F17C6N`          | [torerams](https://github.com/torerams) |
| :file_folder: [`terasic-cyclone-V-gx-starter-kit-test-setup`](https://github.com/stnolting/neorv32-setups/tree/main/quartus/terasic-cyclone-V-gx-starter-kit-test-setup) | Intel Quartus Prime | [Terasic Cyclone-V GX Starter Kit](https://www.terasic.com.tw/cgi-bin/page/archive.pl?Language=English&CategoryNo=167&No=830) | Intel Cyclone V `5CGXFC5C6F27C7N` | zs6mue |
| :file_folder: [`UPduino_v3`](https://github.com/stnolting/neorv32-setups/tree/main/radiant/UPduino_v3)                   | Lattice Radiant     | [tinyVision.ai Inc. UPduino `v3.0`](https://www.tindie.com/products/tinyvision_ai/upduino-v30-low-cost-lattice-ice40-fpga-board/) | Lattice iCE40 UltraPlus `iCE40UP5K-SG48I` | [stnolting](https://github.com/stnolting) |
| :file_folder: [`arty-a7-35-test-setup`](https://github.com/stnolting/neorv32-setups/tree/main/vivado/arty-a7-test-setup) | Xilinx Vivado       | [Digilent Arty A7-35](https://reference.digilentinc.com/reference/programmable-logic/arty-a7/start)                               | Xilinx Artix-7 `XC7A35TICSG324-1L`        | [stnolting](https://github.com/stnolting) |
| :file_folder: [`nexys-a7-test-setup`](https://github.com/stnolting/neorv32-setups/tree/main/vivado/nexys-a7-test-setup)  | Xilinx Vivado       | [Digilent Nexys A7](https://reference.digilentinc.com/reference/programmable-logic/nexys-a7/start)                                | Xilinx Artix-7 `XC7A50TCSG324-1`          | [AWenzel83](https://github.com/AWenzel83) |
| :file_folder: [`nexys-a7-test-setup`](https://github.com/stnolting/neorv32-setups/tree/main/vivado/nexys-a7-test-setup)  | Xilinx Vivado       | [Digilent Nexys 4 DDR](https://reference.digilentinc.com/reference/programmable-logic/nexys-4-ddr/start)                          | Xilinx Artix-7 `XC7A100TCSG324-1`         | [AWenzel83](https://github.com/AWenzel83) |
| :earth_africa: [custom CRC32 processor module for the nexys-a7 boards (**tutorial**)](https://github.com/motius/neorv32-setups/tree/add-custom-crc32-module) | Xilinx Vivado | [Digilent Nexys A7](https://reference.digilentinc.com/reference/programmable-logic/nexys-a7/start)                    | Xilinx Artix-7 `XC7A50TCSG324-1`          | [motius](https://github.com/motius) ([ikstvn](https://github.com/ikstvn), [turbinenreiter](https://github.com/turbinenreiter)) |
| :earth_africa: [neorv32-examples](https://github.com/emb4fun/neorv32-examples) | Intel Quartus Prime | Different Terasic boards  | Different Intel FPGAs | [emb4fun](https://github.com/emb4fun) |


## Setups using Open-Source Toolchains

All setups using open-source toolchains are located in the
[`osflow`](https://github.com/stnolting/neorv32-setups/tree/main/osflow) folder.
See the [README](https://github.com/stnolting/neorv32-setups/blob/main/osflow/README.md)
there for more information how to run a specific setup and how to add new targets.

:bulb: The auto-generated bitstreams built by the [Implementation](https://github.com/stnolting/neorv32-setups/actions/workflows/Implementation.yml)
GitHub workflow can be found in the according **workflow's artifacts**.

| Setup | Toolchain | Board | FPGA | Author(s) |
|:------|:----------|:------|:-----|:----------|
| :file_folder: [`UPDuino-v3.0`](https://github.com/stnolting/neorv32-setups/tree/main/osflow)  | GHDL, Yosys, nextPNR | [UPduino v3.0](https://www.tindie.com/products/tinyvision_ai/upduino-v30-low-cost-lattice-ice40-fpga-board/) | Lattice iCE40 UltraPlus `iCE40UP5K-SG48I` | [tmeissner](https://github.com/tmeissner) |
| :file_folder: [`FOMU`](https://github.com/stnolting/neorv32-setups/tree/main/osflow)        | GHDL, Yosys, nextPNR | [FOMU](https://tomu.im/fomu.html)                                                                            | Lattice iCE40 UltraPlus `iCE40UP5K-SG48I` | [umarcor](https://github.com/umarcor) |
| :file_folder: [`iCESugar`](https://github.com/stnolting/neorv32-setups/tree/main/osflow)    | GHDL, Yosys, nextPNR | [iCESugar](https://github.com/wuxx/icesugar/blob/master/README_en.md)                                        | Lattice iCE40 UltraPlus `iCE40UP5K-SG48I` | [umarcor](https://github.com/umarcor) |
| :file_folder: [`AlhambraII`](https://github.com/stnolting/neorv32-setups/tree/main/osflow)  | GHDL, Yosys, nextPNR | [AlhambraII](https://alhambrabits.com/alhambra/)                                                             | Lattice iCE40HX4K                         | [zipotron](https://github.com/zipotron) |
| :file_folder: [`Orange Crab`](https://github.com/stnolting/neorv32-setups/tree/main/osflow) | GHDL, Yosys, nextPNR | [Orange Crab](https://github.com/gregdavill/OrangeCrab)                                                      | Lattice ECP5-25F                          | [umarcor](https://github.com/umarcor), [jeremyherbert](https://github.com/jeremyherbert) |
| :file_folder: [`ULX3S`](https://github.com/stnolting/neorv32-setups/tree/main/osflow)       | GHDL, Yosys, nextPNR | [ULX3S](https://radiona.org/ulx3s/)                                                                          | Lattice ECP5 `LFE5U-85F-6BG381C`          | [zipotron](https://github.com/zipotron) |
| :file_folder: ChipWhisperer [`iCE40CW312`](https://github.com/stnolting/neorv32-setups/tree/main/osflow) | GHDL, Yosys, nextPNR | **T.B.A.**                                                                                      | Lattice iCE40 UltraPlus `iCE40UP5K-UWG30` | [colinoflynn](https://github.com/colinoflynn) |
| :earth_africa: [`ULX3S-SDRAM`](https://github.com/zipotron/neorv32-complex-setups)          | GHDL, Yosys, nextPNR | [ULX3S](https://radiona.org/ulx3s/)                                                                          | Lattice ECP5 `LFE5U-85F-6BG381C`          | [zipotron](https://github.com/zipotron) |


## Adding Your Project Setup

Please respect the following guidelines if you'd like to add (or link) your setup to the list.

* check out the project's [code of conduct](https://github.com/stnolting/neorv32-setups/tree/master/CODE_OF_CONDUCT.md)
* add a link if the board you are using provides online documentation or can be purchased somewhere
* use the :file_folder: emoji (`:file_folder:`) if the setup is located in this repository; use the :earth_africa:
emoji (`:earth_africa:`) if it is a link to your local project
* please add a `README.md` file to give some brief information about the setup and a `.gitignore` file to keep things clean
* if you like you can add your setup to the [implementation](https://github.com/stnolting/neorv32-setups/blob/main/.github/generate-job-matrix.py)
GitHub actions workflow to automatically generate up-to-date bitstreams for your setup


## Setup-Specific NEORV32 Software Framework Modifications

In order to use the features provided by the setups, minor *optional* changes can be made to the default NEORV32 setup.

* To change the default data memory size take a look at the User Guide section
[_General Software Framework Setup_](https://stnolting.github.io/neorv32/ug/#_general_software_framework_setup)
* To modify the SPI flash base address for storing/booting software application see User Guide section
[_Customizing the Internal Bootloader_](https://stnolting.github.io/neorv32/ug/#_customizing_the_internal_bootloader)
