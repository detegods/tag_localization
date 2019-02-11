The csv includes all read events we collected for the experiments conducted for our paper 
"Estimating Relative Tag Locations based on Time-Differences in Read Events".

The dataset contains the following fields:

experiment_id:  identifier of the experiment
group:          groups experiments with the same properties (setup, experiment,
                tags, iterations)
setup:          "2d" for 2d-setup, 
                "2da" for 2d-asymmetric-setup,
                "3d" for 3d-setup
experiment:     either "walking" or "random"
tags:           nr of tags involved in the experiment
iterations:     nr of iterations
milliseconds:   milliseconds since beginning of the experiment
serial:         the serial number extracted from the epc
rssi:           the measured rssi value

The corresponding ground truth dataset are located in the files 2d.npy, 
2d_asymmetric.npy, and 3d.npy. The files contain the ground truth coordinates 
of the tags, relative to the tag with serial number 0.