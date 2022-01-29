# KitchenSink
A script for switching all running pulseaudio sources to a selected sink. 

I find it very annoying when I switch default audio devices but my currently running sources stay on the old sink. This script allows you to switch the currently selected sink and automatically finds and switches all sources to that sink.


## Usage 
Run ```ksink``` to get a list of available sinks and their ids.

```
$ ksink
Error: Must provide a sink ID
Sink IDs: ['46', '48', '64', '']

46	alsa_output.usb-Kingston_HyperX_Virtual_Surround_Sound_00000000-00.analog-stereo	PipeWire	s16le 2ch 48000Hz	SUSPENDED
48	alsa_output.pci-0000_0f_00.4.analog-stereo	PipeWire	s32le 2ch 48000Hz	SUSPENDED
64	alsa_output.pci-0000_0d_00.1.hdmi-stereo	PipeWire	s16le 2ch 48000Hz	SUSPENDED

```

Run ```ksink <sink id>``` to switch everything but the kitchen sink ;)


## Why Python?
Easier string parsing

