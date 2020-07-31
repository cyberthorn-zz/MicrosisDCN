# MicrosisDCN
MicrosisDCN ver 1.0e based on Raspbian Buster 2019 for Raspberry Pi CM3+ compute module

![](https://raw.githubusercontent.com/cyberthorn-zz/MicrosisDCN/master/MicrosisDCN_banner.jpg)

#### MicrosisDCN_Raspbian_32GB_EagleEye_1_Dec_2019 Download Link (8.84GB .img.xz)
https://drive.google.com/open?id=1v6nKZeUaURGa8a2gkEDMa071WOIIZvcn

#### Start guild read me (1 December 2019)

MicrosisDCN ver 1.0e based on Raspbian Buster 2019
for RPI3 B+, RPI4 and Q-wave EagleEyeSmartCamera 32GB
System contributed by Natthakorn Kasamsumran (Nachod)
Hardware designed by Amornthep Phunsin (Q-wave Systems)

1st step. after flash your 32GB SD-Card or eMMC memory
please run terminal and type "rpi-update" for firmware
update related your SoC on RPi. finally "sudo reboot"

2nd step. update your system package by this command.
"sudo apt-get update && sudo apt-get dist-upgrade"

3nd step. update all pip package by this command.
please type "workon cv" in your terminal windows.
"pip list --outdated --format=freeze | grep -v '^\-e' | cut -d = -f 1  | xargs -n1 pip install -U"

1.) Tensorflow Lite Object Detection Demo
    [Directory path] /home/pi/tensorflow-lite-object-detection
    [Example] Command for initial running.
    $ workon cv
    $ cd tensorflow-lite-object-detection
    $ python3 TFLite_detection_webcam.py --modeldir=Sample_TFLite_model

2.) Computer Vision Raspberry Pi example
    [Directory path] /home/pi/computer-vision-raspberrypi
    [Example] Command for initial running.
    $ workon cv
    $ cd computer-vision-raspberrypi/000-show-pi-camera
    $ python3 app-show-picam.py

3.) Coin Detection, Object face tracking, Camera demo (Peggy)
    [Directory path] /home/pi/example-vision-tensorflow

EagleEye Smart Camera (Q-wave system CO.,LDT.)
https://www.facebook.com/LabviewEmbedded4Arduino/

Microsis DCN Platform (Engineering Chulalongkorn)
https://www.facebook.com/MicrosisDCN/

#### MicrosisDCN ver 1.0e pip install package lists (based on Raspbian Buster 2019-09-26)
absl-py 0.8.1, appdirs 1.4.3, asn1crypto 0.24.0, astor 0.8.0, astroid  2.1.0, asttokens  1.1.13, automationhat 0.2.0, beautifulsoup4 4.7.1, blinker 1.4, blinkt 0.1.2, buttonshim 0.0.2, cachetools 3.1.1, Cap1xxx 0.1.3, certifi 2018.8.24, chardet 3.0.4, Click 7.0, colorama 0.3.7, colorzero 1.1, cookies 2.2.1, cryptography 2.6.1, cv 1.0.0, cycler 0.10.0, decorator 4.3.0, docutils 0.14, drumhat 0.1.0, entrypoints 0.3, envirophat 1.0.0, ExplorerHAT 0.4.2, Flask 1.0.2, fourletterphat 0.1.0, gast 0.3.2, google 2.0.2, google-api-core 1.14.3, google-api-python-client 1.7.11, google-auth 1.7.0, google-auth-httplib2 0.0.3, google-cloud 0.34.0, google-cloud-vision 0.40.0, google-pasta 0.1.8, googleapis-common-protos 1.6.0, gpiozero   1.5.1, grpcio 1.25.0, guizero 0.6.0, h5py 2.10.0, html5lib 1.0.1, httplib2 0.14.0, idna 2.6, imageio 2.6.1, imutils 0.5.3, ipykernel 4.9.0, ipython 5.8.0, ipython-genutils 0.2.0, isort 4.3.4, itsdangerous 0.24, jedi  0.13.2, Jinja2 2.10, joblib 0.14.0, jupyter-client 5.2.3, jupyter-core 4.4.0, Keras 2.3.1, Keras-Applications 1.0.8, Keras-Preprocessing 1.1.0, keyring 17.1.1, keyrings.alt 3.1.1, kiwisolver 1.0.1, lazy-object-proxy 1.3.1, logilab-common 1.4.2, lxml 4.3.2, Markdown 3.1.1, MarkupSafe 1.1.0, matplotlib 3.0.2, mccabe  0.6.1, microdotphat 0.2.1, mote 0.0.4, motephat 0.0.2, mypy 0.670, mypy-extensions 0.4.1, networkx  2.4, nudatus 0.0.4, numpy 1.17.4, oauthlib 2.1.0, olefile 0.46, pandas 0.25.3, pantilthat 0.0.7, parso 0.3.1, pbr 5.4.3, pexpect 4.6.0, pgzero 1.2, phatbeat 0.1.1, pianohat 0.1.0, picamera 1.13, pickleshare 0.7.5, picraft 1.0, piglow 1.2.5, pigpio 1.44, Pillow 5.4.1, pip 19.3.1, prompt-toolkit 1.0.15, protobuf  3.10.0, psutil 5.5.1, pyasn1 0.4.7, pyasn1-modules 0.2.7, pycairo 1.16.2, pycodestyle 2.4.0, pycrypto  2.6.1, pyflakes 2.0.0, pygame 1.9.4.post1, Pygments 2.3.1, PyGObject 3.30.4, pyinotify 0.9.6, PyJWT 1.7.0, pylint 2.2.2, pyOpenSSL 19.0.0, pyparsing 2.2.0, pyserial 3.4, python-apt 1.8.4, python-dateutil  2.7.3, pytz 2019.3, PyWavelets 1.1.1, pyxdg 0.25, PyYAML 5.1.2, pyzmq 17.1.2, qtconsole 4.3.1, rainbowhat 0.1.0, requests 2.21.0, requests-oauthlib 1.0.0, responses 0.9.0, roman 2.0.0, RPi.GPIO 0.7.0, rsa 4.0, RTIMULib 7.2.1, scikit-image 0.16.2, scikit-learn 0.21.3, scipy 1.3.2, scrollphat 0.0.7, scrollphathd  1.2.1, SecretStorage 2.3.1, semver 2.0.1, Send2Trash 1.5.0, sense-emu 1.1, sense-hat 2.2.0, setuptools 40.8.0, simplegeneric 0.8.1, simplejson 3.16.0, six 1.12.0, skywriter 0.0.7, sn3218 1.2.7, soupsieve 1.8, spidev 3.3, ssh-import-id 5.7, stevedore 1.31.0, tensorboard 1.13.1, tensorflow 1.13.1, tensorflow-estimator 1.14.0, termcolor 1.1.0, tflite-runtime 1.14.0, thonny 3.2.0, tornado 5.1.1, touchphat 0.0.1, traitlets 4.3.2, twython 3.7.0, typed-ast 1.3.1, uflash 1.2.4, unicornhathd 0.0.4, uritemplate 3.0.0, urllib3 1.24.1, virtualenv 16.7.7, virtualenv-clone 0.5.3, virtualenvwrapper 4.8.4, wcwidth 0.1.7, webencodings 0.5.1, Werkzeug 0.14.1, Wheel 0.32.3, wrapt 1.11.2  

#### N. Kasamsumran, P. Chanchaithong, N. Wattanamongkhol, W. Pora and S. Pumrin, "Applying Faster R-CNN for Hematocytes Detection on Compound Microscope with Image Sensor Device and Multiple GPU Computation," 2020 8th International Electrical Engineering Congress (iEECON), Chiang Mai, Thailand, 2020, pp. 1-4, doi: 10.1109/iEECON48109.2020.229490.
