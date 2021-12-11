# JetsonRocksSeashells
AI to detect and classify rocks and seashells for the Jetson AI Specialist Certificate, sought during the MAE/ECE 148 class at UCSD.

The scripts in this Jetson Inference-based repository detect and classify rocks and sea shells. More developed and advanced AI tools like this one could be used to differentiate between rocks and shells in marine environments, either for use in aquaculture (i.e. harvesting mussels and clams), or to identify otherwise well-camoflauged shellfish underwater for conservation purposes.

# Installation
Instructions to install Jetson Inference from Github:

```
sudo apt-get update
sudo apt-get install git cmake libpython3-dev python3-numpy nano scrot python3-pip
git clone --recursive https://github.com/dusty-nv/jetson-inference
cd jetson-inference
mkdir build
cd build
cmake ../
make -j$(nproc)
#WHEN ASKED CHOOSE ALL MODELS OBJECT DETECTION
sudo make install
sudo ldconfig
```

Clone the Git Repository:

```
git clone https://github.com/LiamEFowler/JetsonRocksSeashells
```

This code is designed for a USB-camera. Follow instructions in the Hello AI World video tutorials to replace the /dev/video0 with the correct camera formatting if you are using a different camera.

# Run in terminal
You should be in the jetson-inference directory you cloned and running the docker container with the JetsonRocksSeashells mounted into it (see https://github.com/dusty-nv/jetson-inference/blob/master/docs/aux-docker.md#mounted-data-volumes)
```
python3 my-detection.py
```
# Video
See "Jetson AI Specialist Screen Recording.mp4" in this repository.

Enjoy!

Special thanks to Johannes Diehm for inspiration.
