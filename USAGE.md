# USAGE

Examples include 
- "Evening map", either all-sky or binocular-grade maps covering the horizon with 8 portrait- or 4 landscape-oriented maps. Add a landscape polygon from Stellarium (e.g. created by Peakfinder) to read location and horizon profile. Create them systematically without planets for years of use, or with planets just for a particular date.
- systematic sky coverage in J2000.0 atlas style with various combinations of --fieldsize/--limit--dso/--limit-star and labeling options.
- search maps for favourite deep-sky objects or stars. Try the __allmessier__ target for a personal Messier album.
- TBD: singular constellation targets
- TBD: Planet/comet/asteroid trails


It may be useful to create several personal *.conf files for your tasks. They are applied in the sequence as listed on the command line: Probably you will find your personal favourite set of colors. Or have 2 or even 3 sets, one for printable black on white maps (or one in pure black and one with mixed colors) and one with black background for display graphics.  Then you may have different line widths. and of course, various levels of detail (magnitude limits, DSO catalogs, label options)  for varying fieldsizes, e.g. in files called fs2.conf, fs5.conf, fs15.conf, fs25.conf, fs45.conf, fs70.conf, fs95.conf, fs150_ls.conf. Here the short option -c is handy.


python bin\fchart3 -c light_colors.conf -c fs15.conf M20

python bin\fchart3 -c light_colors.conf -c fs95.conf "h:270,45,West"

Specify a Stellarium horizon without trailing path delimiter! Specify time as "now" or as full ISO-8601 timestring like "2026-01-02T21:15:00Z", "2026-01-02T21:15:00+01:00", or any part of it that uses "today" Note that a Stellarium landscape sets a timezone for you, but you can override it. 

python bin\fchart3 -c light_colors.conf -c fs150_ls.conf --stellarium-landscape "D:\Stellarium\landscapes\my_site" -cs horizontal -t "T22:00+01:00" "h:270,45,West"


