When collecting altitude data from a running vehicle,
the sensor data collected can often go haywire,
especially when there's no connectivity to the cloud
we see a drastic change in its values.

A gradual or steady change might be explicable accounting
for the path traveled by the vehicle however a sudden
drastic change like the data I've got here is not justified.

We cannot employ a simple peak identifier or a standard IQR
treatment of outliers across all kinds of data, especially
If there's an uptrend or downtrend in the altitude.One might
have to come up with a more generic yet optimal approach to
handle this scenario.

I have used the sliding window mean technique here to calculate
the shift in the altitude from its last window's mean value to 
capture the oddity or the difference. If the difference is above
or below a particular threshold, one can pick the odd signal that
doesn't fit its nearest group and it can be removed or replaced
with the nearest group's mean for better oddity treatment.

However, a problem arises when there are more consecutive haywire
values, which then have to be handled differently.
