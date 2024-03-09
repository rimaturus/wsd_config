## How to install Ubuntu 22 on WSL with Nvidia access
# 1) Preparing Windows
1) Download the latest Nvidia GPU driver: https://www.nvidia.com/Download/index.aspx _{select the proper ones for your graphics card}_

2) Download CUDA Toolkit: [direct link for Windows 11: https://developer.download.nvidia.com/compute/cuda/12.4.0/local_installers/cuda_12.4.0_551.61_windows.exe ]

3) Install wsl on cmd or Powershell: 
    i)      `wsl.exe --install`
    ii)     `wsl.exe --update`
    After that, search and click on the Ubuntu Icon on your "start" section, it will start the Ubuntu configuration

## 2) Setting up Ubuntu
1) Move this folder inside your ubuntu home (drag and drop in the Linux -> Ubuntu -> home -> username folder that you can find on your File Explorer)
2) Open the Ubuntu terminal and launch the script: `sudo bash configure_wsl_nvidia.sh`
It will configure the Cuda toolkit inside your wsl and install all the necessary dependencies and docker.

## FONTI:
1) https://github.com/ashishpatel26/Cuda-installation-on-WSL2-Ubuntu-20.04-and-Windows11?tab=readme-ov-file
2) https://developer.nvidia.com/cuda/wsl
3) https://docs.nvidia.com/cuda/wsl-user-guide/index.html
