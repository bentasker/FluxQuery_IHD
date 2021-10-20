FluxQuery Based Energy Usage Graphs
=======================================

This is a set of example HTML and Javascript designed to query energy-usage information out of an [InfluxDB](https://www.influxdata.com/products/influxdb/) instance (actually, it should work with [InfluxDB Cloud](https://www.influxdata.com/products/influxdb-cloud/) too) using [Flux](https://docs.influxdata.com/flux/v0.x/), and graph it out using [Flot](http://www.flotcharts.org/).

These were used to [create an In-Home-Display](https://www.bentasker.co.uk/blog/house-stuff/744-creating-a-ihd-to-view-energy-usage).


### Notes

- If you're going cross-origin to reach your InfluxDB instance, you'll need to make sure appropriate CORS headers are returned in response to `OPTIONS` requests (the queries use `POST` so will trigger pre-flight checks)
- There's plenty of tidying and DRYing that could be done, especially in the HTML and CSS
- This runs more than happily on a [Raspberry Pi based kiosk](https://www.bentasker.co.uk/documentation/linux/687-building-a-raspberry-pi-based-music-kiosk) sat on a kitchen counter.
- If you intend to use it, you'll need to set the value of var `influxdb` in `graph.html`


----

## Copyright

Copyright (c) 2021 B Tasker

Released under the [Creative Commons Attribution (CC BY) license](https://creativecommons.org/licenses/by/4.0/)
