# Data set of 802.15.4 data captures

## Context

This data has been created as part of a thesis for the master degree Software Engineering. The research that the data is part of aims to determine whether the different signals can be classified correctly by convolutional neural networks. The data has been placed on github to make sure it does not go lost, but also to make the research auditable and allow data to be inspected by those reviewing the thesis.

## Technical properties of the data

The data has been captured using an ADALM Pluto SDR.

In line with the intended research setup, a specific frame type was selected for each device. For example for the Innr smart plug the "Data" frame has been selected.

The initial data captures were several seconds in size and contained multiple signal spikes. A combination of Wireshark, GNU radio and Universal radio hacker has been used to extract the intended frame types. Each signal in this github repository represents one 802.15.4 frame for a specific device.

The data is stored in the github repository as interleaved IQ data. This data will be further (pre-)processed before it is used as input for the CNNs. Only the "raw" data is shared via this repository.

The number of data frames collected for each device differs. This was because the aim was to arrive at 1000 data patches for each device, of 1024 data points each. Because the size per frame per device is different, different numbers of samples were required to arrive a the same number of data patches.

Sample rate used is 4MHz for all devices. Bandwidth was 2.5 MHz for all devices.

Devices:

+ Philips Hue bridge (Frequency used was 2.425 GHz)
+ Innr smart plug (Frequency used was 2.425 GHz)
+ AEOTEC open/close door sensor (Frequency used was 2.405 GHz)
+ Endress+Hauser SWG50 FieldGate (WirelessHart; various channels in the 2.4x GHz range)


## License

This dataset is licensed under the Open Data Commons Attribution License v1.0 (ODC-BY: https://opendatacommons.org/licenses/by/1-0/). Which means you are free to share/copy/distribute as long as you attribute public use or works produced from the dataset in the manner specified in the license (giving appropriate credit, providing a link to the license and indicating if changes were made).

