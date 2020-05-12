Gonewild Archiver (clone of Gonewilder)
==========

This fork of the "gonewilder" archive script is also a content downloader, but is geared towards the "Gonewild" subreddits of reddit. At present, this pulls on a loop from the top 100 hottest posts of the following subreddits:

* petitegonewild
* repressedgonewild
* militarygonewild
* gonewild
* gonewildcurvy
* asiansgonewild
* gonewildplus
* treesgonewild
* workgonewild
* altgonewild
* gifsgonewild
* gonewildcolor
* dykesgonewild
* gonewildsmiles
* bigboobsgonewild
* gonewildmetal

Please submit a request or issue if you'd like other subs added.


Installing
==========

Requires:
* Python
* Python Imaging Library (PIL)
* SQLite3

Optional:
* Apache (for web interface only, BUT KEEP IN MIND, "serve.py" will also run a python webserver on port 7070)
** Files in root (`.`) and `py` directories need to be CGI Executable in Apache

Install dependencies on Debian: 10 (buster)
==========================================

```bash
apt-get install python2.7-dev python-tk python-setuptools python-pip python-dev libjpeg9-dev libjpeg9 tcl-dev tcl zlib1g-dev zlib1g libsnack2-dev tk8.6-dev libwebp-dev libwebp6 vflib3-dev libfreetype6-dev libtiff5-dev libjbig-dev
pip install pillow
```

Executing
=========

To start the application, execute `Gonewild.py` from the `./py/` directory:

```bash
python Gonewild.py
```

With no arguments, this will start an infinite loop in the current window, which checks for and downloads new content. It is best to run in screen.

For help / other options, try:

```bash
python Gonewild.py --help
```

Additional Notes
=========

This does come with python based web server script that will organize the files into a nice website for easy browsing, searching, and adding of specific girls.
