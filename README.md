# OpenPose_Install_Python

[OpenPose GitHub](https://github.com/CMU-Perceptual-Computing-Lab/openpose)

[Installation](https://github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/doc/installation.md)

- Download the source code
- Download and install CMAKE and VS2015(with CUDA8.0)
- Open CMAKE, specify the source code and the build dir.
- Click `Configure`, select `Visual Studio 14 2015 Win64`, and click Finish
  - Any errors encountered, check your VS environment (may be you have to reinstall **all** of your vs components) and log file
  - May be you would encounter `cl.exe` and `rc.exe` problems
- If cmake passed, check the cuda dir. and select `BUILD PYTHON` box, and click `Generate`
- Then click `Open Project`, then the VS2015 would be open
- Switch `Debug` to `Release` and select `x64`, then press `F5` to run the project
- The project start running after compiling for a while, and you would see your camera begin to work
- After compiling, you would have to build the project `_openpose`, right click it, and click `Build`


