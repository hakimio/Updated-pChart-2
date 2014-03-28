Updated-pChart-2
================

pChart 2.1.4 updated with changes from dakota/pchart plus some other minor fixes:
Changes from dakota repository:
o Proper php 5.3 "__construct" constructors.
o Added 'AxisYFont' parameter for drawScale function (array with R, G, B, Alpha, FontName and FontSize parameters)
o Added 'AxisYDistance' parameter for drawScale function (the distance to move axis name from the axis)
o Replaced function_exists with is_callable to check if custom axis format function was specified correctly
o Replaced preg_split with explode - explode is faster as it doesn't need to build regexp
o $SerieOrder in drawStackedAreaChart function is now correctly initialised as array

Other changes:
o All the changes from pChart 2.1.4 version (dakota's changes were applied only on version 2.1.3)
o Added 'MaxWidth' parameter to drawBarChart function (specifies maximum bar width)
o Corrected $SLabelxRotation to $XLabelsRotation in drawScatterScale function
o Initialized $XLast and $YLast in drawSpline function