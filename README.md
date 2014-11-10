obwaita
=======

Adwaita for Openbox (ish)

Obwaita, is an attempt to get openbox to play nice with Adwaita, the default
gtk3 theme.

It's not exactly a feeble attempt at a port as it seemed futile to attempt to 
port the mutter decorations, it's basically a last gasp effort to allow me to 
keep using openbox with a modern theme without it sticking out like a relic.

HERE BE DRAGONS

* The handles are disabled by default
* Menu borders are disabled by default
* It's probably best to use a composite manager like compton or xcompmgr or 
  something, I use these settings with compton:

  shadow-radius = 6;
  shadow-offset-x = -9;
  shadow-offset-y = -6;
  shadow-opacity = 0.5;
  shadow-exclude = ["_GTK_FRAME_EXTENTS@:c"];

  They more or less mimic the client side window shadows from Adwaita and will 
  stop the ugly double shadow problem
