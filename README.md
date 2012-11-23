openlayers-timeslider
=====================

A plugin for OpenLayers used for displaying a timeslider for layers with a time dimension.

If multiple layers are shown the plugin merges that the available times for a the layers. The plugin does not contain
any logic for trying to "fill the gaps" if some times are not available for all layers.

The plugin depends on the Slider component in jQuery UI version 1.8.x and will not work with out it.


## Usage

To use, just include the TimeSlider.js file and add it as part of the map controllers like this:

    var timeSliderDiv = document.getElementById('timesliderId');
    var map = new OpenLayers.Map({ div: "map",
                                   controls : [ new OpenLayers.Control.TimeSlider({ div : timeSliderDiv } ),],
                                });
