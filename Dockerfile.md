# Begin the docker 

Docker of pop-bread to run
  $ nvidia-docker run -it --rm --ipc=host --shm-size=1g --ulimit memlock=-1 --ulimit stack=67108864 -v $PWD://work/model/ xuandocker bash

The pop-bread model to run
 
  $ python3 main.py

# The dmesg

ImportError: No module named 'easygui'

  $ pip3 install easygui

ImportError: No module named '_tkinter'

  $ apt-get update
  $ apt-get install python3-tk
  
NameError: name 'opencvYOLO' is not defined

  $ apt-get install libopencv-dev

ImportError: No module named 'yoloOpencv'

  $ wget https://github.com/ch-tseng/traffic/blob/master/yoloOpencv.py
  
ImportError: No module named 'imutils'
  #  

ImportError: No module named 'PIL'

  $







