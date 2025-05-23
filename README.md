## 🚀 How to Use
### 🛠️ Prerequisites

#### ✅ Install OpenCV with Contrib Modules (C++)

📥 OpenCV with Contrib Modules (C++) :

https://github.com/opencv/opencv_contrib

     # Step #1 - Install dependencies
     sudo apt update && sudo apt install -y cmake g++ libgtk-3-dev libtbb-dev
     
     # Step #2 - Clone OpenCV and contrib
     cd ~
     git clone https://github.com/opencv/opencv.git
     git clone https://github.com/opencv/opencv_contrib.git
     
     # Step #3 - Build and install
     cd opencv && mkdir build && cd build
     cmake -D CMAKE_BUILD_TYPE=Release \
           -D CMAKE_INSTALL_PREFIX=/usr/local \
           -D OPENCV_EXTRA_MODULES_PATH=~/opencv_contrib/modules ..
     make -j$(nproc)     
     sudo make install
     pkg-config --modversion opencv4


#### ✅ Install RealSense SDK

📥 Intel RealSense SDK : 

https://github.com/IntelRealSense/librealsense/blob/master/doc/installation.md

### ⚙️ Build and Run

     # Step #1 - Clone this repo
     git clone https://github.com/ichsanyudika/REALSENSE-SEGMENT.git
     
     # Step #2 - Build
     cd REALSENSE-SEGMENT
     mkdir build && cd build
     cmake ..
     make
     
     # Step #3 - Run the application
     ./cam

#### 📸 **Results**

![](output/output.png)
