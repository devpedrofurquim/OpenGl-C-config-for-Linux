
# OpenGl C config for Linux OS 

*work in progress* | *all the code written in C*

Hello! For now I only have the code to open a window on the Linux OS with the shared libraries Glew and Glfw.

This configuration is the equivalent of the <windows.h> shared library for Windows, which works only on windows.






## Run Locally

Clone the project

```bash
  git clone https://git@github.com:devpedrofurquim/opengl-c-config-for-linux.git
```

Go to the project directory

```bash
  cd OpenGl-C-config-for-Linux 
```

Update your Linux and install OpenGl and dependencies

```bash
  sudo apt-update
```
```bash
sudo apt-get install cmake pkg-config
```
```bash
sudo apt-get install mesa-utils libglu1-mesa-dev freeglut3-dev mesa-common-dev
```
```bash
sudo apt-get install libglew-dev libglfw3-dev libglm-dev
```
```bash
sudo apt-get install build-essential libxmu-dev libxi-dev libgl-dev
```
```bash
sudo apt-get install libao-dev libmpg123-dev
```
Download the GLFW library on this link https://sourceforge.net/projects/glfw/files/glfw/3.0.4/glfw-3.0.4.tar.gz/download

Go to the directory of the file and extract it

```bash
  cd Downloads
```
```bash
  tar xzvf glfw-3.0.4.tar.gz
```
Install the GLFW library
```bash
  cd glfw-3.0.4
```
```bash
  mkdir build
```
```bash
  cd build
```
```bash
  cmake ../
```
```bash
  make && sudo make install
```
These comands above will install the library.

Now let's install the GLEW library.

Download the library on this link https://sourceforge.net/projects/glew/files/glew/2.1.0/glew-2.1.0.zip/download

Go to the directory of the file and extract it.

Then run this command on the extracted folder
```bash
  sudo make install
```
It will will attempt to install GLEW into /usr/include/GL and /usr/lib.
## Usage

### Now you must be able to open a window on Linux with 0 errors. Let's try it.

Run the breakout executable file 
``` bash
    ./breakout
```
A empty window will show up on your screen, press ESC to close it. Now it's working. If you have any issues let me know.
