---
permalink: /projects/deep_learning/neural_fpga/
title: "Neural FPGA"

sidebar:
  nav: "docs"

layout: archive

classes: wide
---


<i class="fab fa-fw fa-github"></i> [**Neural FPGA GitHub**](https://github.com/JdeRobot/neuralFPGA).
{: .notice--info}


Neural FPGA project goal is to produce custom hardware able to do inference over generic neural networks using only open source tools. In order to test our hardware designs we rely on hardware simulations and FPGAs.

Hardware simulation open source tools have been available since long time (see [Verilator](https://www.veripool.org/wiki/verilator), [Icarus Verilog](http://iverilog.icarus.com/)), but open source tools to generate bitstreams for FPGAs were lacking until recent. Project [IceStorm](http://www.clifford.at/icestorm/) was the first complete tool to program a commercially available FPGA, the [Lattice iCE40](http://www.latticesemi.com/Products/FPGAandCPLD/iCE40.aspx). Following, the project [prjtrellis](https://github.com/SymbiFlow/prjtrellis) is documenting the bitstream format for the more capable [Lattice ECP5](http://www.latticesemi.com/Products/FPGAandCPLD/ECP5). And others are comming.

On this project we won't focus on specific FPGAs, but because we would like to run our designs on real hardware we will try to fit our designs to available hardware with open source tools. This for the time being will be Ice40 and ECP5 from Lattice.

The main output of this project are cores that can do inference on generic neural networks trained with TensorFlow.