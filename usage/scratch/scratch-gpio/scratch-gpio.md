# Scratch GPIO


- --
## Appendix: Enabling and disabling the GPIO server.
In normal use you shouldn't need to enable the GPIO server as by default it is enabled but stopped. We can change this by adding  a line to the init file (in the HOME directory we can have a file named `.scratch.ini` - the initial dot is important to make it a hidden unix file)
Simply add a line
`gpioserver=X`
to the file, where X is:
   - `0` - to disable the GPIO server, preventing users or loaded projects from using it.
   - `1` - to enable the GPIO server but leave it turned off; this is the default when there is no .scratch.ini file
   - `2` - to both enable and start the server, perhaps useful in a classroom when the lesson will be about GPIO use

Note that the older mesh/network server setup is currently semi-hidden under the Share menu - you have to hold down the shift key whilst opening that menu.