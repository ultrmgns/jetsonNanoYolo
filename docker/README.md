# Instructions on how to run YOLO v10/11 inference on NVidia Jetson Orin Nano/Nano NX

First execute this directly on the Jetson host:
```
xhost +local:docker
```

It will enable EGL streaming from the container.

Second, pull the and run the ATN custom container

```
sudo docker run --runtime nvidia -it --rm -p 8888:8888 -p 7860:7860 -p 7866:7866 -v $(pwd):/app --device /dev/video0 --device /dev/video1 -v /tmp/argus_socket:/tmp/argus_socket -v /etc/enctune.conf:/etc/enctune.conf -v /usr/lib/aarch64-linux-gnu/tegra:/usr/lib/aarch64-linux-gnu/tegra -v /usr/lib/aarch64-linux-gnu/gstreamer-1.0:/usr/lib/aarch64-linux-gnu/gstreamer-1.0 -v /usr/src/jetson_multimedia_api:/usr/src/jetson_multimedia_api --privileged zelias/yolov10atn:v5
```
This includes PyTorch with CUDA support, OpenCV with CUDA and GStreamer support

Enter the container's shell (use sudo docker ps to see the id):
```
docker exec -it <id> bash
```

Inside the container, check gstreamer for errors:
```
gst-inspect-1.0 nvarguscamerasrc
```

Test EGLDisplay inside the container:
```
glxinfo | grep "OpenGL version"
```
If it's not installed or you have errors, run:
```
apt-get update && apt-get install -y mesa-utils 
```

