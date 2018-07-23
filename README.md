# OpenPose_Install_Python

## Source

[OpenPose GitHub](https://github.com/CMU-Perceptual-Computing-Lab/openpose)

[Installation](https://github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/doc/installation.md)

## Steps
- Download the source code
- Download and install CMAKE and VS2015(with CUDA8.0)
- Open CMAKE, specify the source code and the build dir.
- Click `Configure`, select `Visual Studio 14 2015 Win64`, and click Finish
  - Any errors encountered, check your VS environment (may be you have to reinstall **all** of your vs components) and log file
  - May be you would encounter `cl.exe` and `rc.exe` problems
  - ![cmake]()
- If cmake passed, check the cuda dir. and select `BUILD PYTHON` box, and click `Generate`
- Then click `Open Project`, then the VS2015 would be open
- Switch `Debug` to `Release` and select `x64`, then press `F5` to run the project
- The project start running after compiling for a while, and you would see your camera begin to work
- After compiling, you would have to build the project `_openpose`, right click it, and click `Build`


## Problems
- [rc.exe](https://stackoverflow.com/questions/14372706/visual-studio-cant-build-due-to-rc-exe)
  - Runtime C++ compiler, it wouldn't install to your computer during vs2015 installation
- cl.exe
  - c++ compiler, you may not install it during vs2015 installation, then modify your installer, and add it into your VS

