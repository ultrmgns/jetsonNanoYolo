# Configuring Jetson Orin Nano to have OpenCV with CUDA, PyTorch with CUDA, GStreamer, torchvision and YOLOv10/11
YOLO v10's performance bellow Python 3.10 is far too slow, so start with installation of Python version 3.10 or 3.11.
Then, check if you have cudNN and if OpenCV is compiled with CUDA:

```sh
sudo pip3 install -U jetson-stats
sudo reboot
jtop 
```

Go to Info tab and see the information.\
Alternatively you can use the jetsonUtilities:

    git clone https://github.com/jetsonhacks/jetsonUtilities

    cd jetsonUtilities
    python jetsonInfo.py

Side note: for `JetPack =>6`, it will show "JetPack UNKNOWN" (36.x.x)


## Compiling OpenCV with CUDA:
I took care for most of the errors that occur with this script:
`OpenCV-4.10.0_2.sh`

Check the part number on your Jetson device to make sure of the model. 
The script checks the device ID and compiles the wheel and installs it.
If you need to, change the model name in the beginning of the script to correspond from the information from the info above (in this section):

```sh
# Check if the model information contains "Jetson Nano Orion"
        echo ""
        if [[ $model == *"Orin"* ]]; then
            echo "Detecting a Jetson Nano Orin."
```

If it fails at some point: `sudo rm -r ../opencv/build`
And check what the error is before re-compiling.

Don't forget to check if Architecture corresponds inside the script:
- For Orin Nano and NX, arch should be 8.7
- For older: 5.3

## Compiling PyTorch with CUDA enabled:

Version Compatibility Matrix for PyTorch
This table contains the history of PyTorch versions, along with compatible domain libraries.

```
PyTorch Version     torchvision     torchtext	    torchaudio	PyTorch Release Date
2.4.0	            0.19.9	        0.18.0	        2.4.0	    07/24/2024
2.3.0	            0.18.0	        0.18.0	        2.3.0	    04/24/2024
2.2.0	            0.17.0	        0.17.0	        2.2.0	    01/30/2024
2.1.0	            0.16.0	        0.16.0	        2.1.0	    10/04/2023
2.0.0	            0.15.1	        0.15.1	        2.0.1	    03/15/2023
1.13.0	            0.14.0	        0.14.0	        0.13.0	    10/28/2022
1.12.0	            0.13.0	        0.13.0	        0.12.0	    06/28/2022
```

Easiest way is to download manually a pre-built wheel for PyTorch with CUDA enabled.
Start from this link:
https://developer.download.nvidia.com/compute/redist/jp/

Choose the JetPack version, install it:
```sh
wget https://developer.download.nvidia.com/compute/redist/jp/v60/pytorch/torch-2.4.0a0+f70bd71a48.nv24.06.15634931-cp310-cp310-linux_aarch64.whl
pip install torch-2.4.0a0+f70bd71a48.nv24.06.15634931-cp310-cp310-linux_aarch64.whl
```

After that is done, you have to install torchvision, do it like this:

    pip install torchvision==0.19.9 --no-deps

(for no dependancies, otherwise it will automatically uninstall torch and install the cpu-only version)

After this, use the included Python workbooks to check if Torch is installed with CUDA enabled with its GPU name, and if OpenCV has CUDA enabled.
systemChecks.ipynb

After that, you can start object detection from the YOLOv10n.ipynb workbooks (tested and working above 50 fps on Orin Nano 8Gb).


