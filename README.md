You will need OpenCV, Festival and pi-blaster installed for this to work:

sudo apt-get install python-opencv festival

pi-blaster is a manual install: https://github.com/sarfata/pi-blaster/

The text files named hi and bye are the files from which Festival speaks
when a face is detected (hi) and when the face leaves the screen (bye).
You can modify these files as necesary to get the desired speaking for
each face event.  Be aware that using pi-blaster for the servos means
you can't use the analog audio anymore - it's busy generating the PWM
signals for the servos.  Audio must be via HDMI for this to work.  This
is a setback for now, sorry.

I used the OpenCV code on this webpage: 
http://www.technolabsz.com/2013/03/how-to-easily-install-opencv-on.html

Included is the Python script and the human face XML from which the
OpenCV uses to identify the faces.  I modified the facedetect.py script
to work with the servos and festival output - this is the script that
you have now from this Github repo.

Any questions please feel free to ask.

