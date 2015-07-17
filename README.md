# trilegaldiagnostics
An ongoing repo to aide in displaying trilegal catalogs

##Install

<pre>pip install trilegaldiagnostics</pre>

##Basic usage

<pre>$ color_by_arg trilegalfile xcolumn ycolumn ccolumn</pre>

For example, if you want a CMD colored in 8 bins by stage:

<pre>$ color_by_arg trilegalfile -b 8 F606W-F814W F814W stage</pre>

If you want it colored by C/O but only values from 0.5-2 and you want a pdf instead of a png:

<pre>$ color_by_arg trilegalfile -v 0.5,2 -e pdf -b 8 F606W-F814W F814W C/O</pre>

You can also make my default 3x2 grid of plots using <code>-a</code> flag.

For other options (like setting the <code>xlim</code>, <code>ylim</code>, and <code>colorbar</code> limits) see

<pre>color_by_arg -h</pre>
