# Trackpad on Umax Vision book 13w FLEX

Under Fedora the trackpad is not recognized, 

'''bash
sudo modprobe -r psmouse && sudo modprobe psmouse
'''

and 

''' bash
sudo modprobe -r psmouse && sudo modprobe psmouse proto=imps
'''

does nothing,

on Debian isn't recognized too, nothing in the output of:

'''bash
xinput list
'''

