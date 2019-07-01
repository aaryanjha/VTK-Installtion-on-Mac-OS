# VTK-Installtion-on-Mac-OS

## Downloading vtk

- First download the vtk source file from the link given below

```
https://www.vtk.org/files/release/8.2/VTK-8.2.0.zip
```
- Create a folder named `vtk` in the directory `/usr/local/`
- Inside the folder `vtk`, create two more folders and name it as `src` and `build`
- Copy all the fiels and folders from the vtk source folder that you have downloaded and paste it in the `src` folder in `/usr/local/vtk/` folder
## Downloading cmake
- Now install the cmake gui using homebrew by making use of following commands
```
brew install cmake
```
- Now add the cmake path to the command line by running the following command in terminal
```
 PATH="/Applications/CMake.app/Contents/bin":"$PATH"
```
- Now you are all done to install th vtk
## Installing vtk
- Go to the vtk build folder using following coomand in terminal(it may differ)
```
cd /usr/local/vtk/build
```
- Now you are on the build folder inside the vtk, run the following command to configure
```
ccmake .
```
- Now Select your prompt and configure by pressing `c`
- Configure it twice
- After that press `g` to generate
- Now you have successfully generated the build file
- Now run the following command to make(it would probably take half an hour)
```
make -j4
```
- You vtk is installed
- trying running different examples from the link given below by following the instruction over their on the link
```
https://vtk.org/Wiki/VTK/Examples/Cxx
```
