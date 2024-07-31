# Data set of 802.15.4 data captures

## Context

This data has been created as part of my thesis for the master degree Software Engineering. The research that the data is part of aims to determine whether the different signals can be classified correctly by several convolutional neural networks. The data has been placed on github to make sure it does not go lost, but also to make my research auditable and allow data to be inspected by those reviewing the thesis.

## Technical properties of the data

The data has been captured using an ADALM Pluto SDR.

As part of the research setup, a specific frame type was selected for further research for each device. For example for the Innr smart plug the "Data" frame has been selected as input for further research. Initial data captures of several seconds contained multiple signal spikes. A combination of Wireshark, GNU radio and Universal radio hacker has been used to select the proper frame types. Each signal in this github repository represents one 802.15.4 frame for a specific device.

On the data no further pre-processing has taken place; this is done locally as part of the research. The number of frames per device differs because the size per frame per device is different and the aim was to arrive at 1000 data patches per device of 1024 data points each.

Sample rate used is 4MHz for all devices. Bandwidth was 2.5 MHz for all devices.

Devices:

+ Philips Hue bridge (Frequency used was 2.425 GHz)
+ Innr smart plug (Frequency used was 2.425 GHz)
+ AEOTEC open/close door sensor (Frequency used was 2.405 GHz)


## License

This dataset is licensed under the Open Data Commons Attribution License v1.0 (ODC-BY: https://opendatacommons.org/licenses/by/1-0/). Which means you are free to share/copy/distribute as long as you attribute public use or works produced from the dataset in the manner specified in the license (giving appropriate credit, providing a link to the license and indicating if changes were made).

