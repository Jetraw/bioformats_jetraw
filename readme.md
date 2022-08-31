# Jetraw Fiji Bio-Formats
This is the Fiji Bio-Formats plug-in for Jetraw. With this Bio-Formats plug-in version you will be able to read Jetraw compressed TIFF files using your current Fiji installation. For more info visit https://www.jetraw.com/

## Requirements
- **Jetraw installed** on a Windows, Linux or macOS computer.<br/>
*Note:* if you do not have Jetraw installed visit https://www.jetraw.com/downloads/software and for usage information https://github.com/Jetraw/Jetraw
- **Fiji installed** with Bio-Formats plug-in (accepted versions 6.5.1, 6.6.0, 6.6.1, 6.7.0, 6.8.0, 6.8.1, 6.9.0, 6.9.1, 6.10.0 and 6.10.1)<br/>
*Note:* if you do not have Fiji installed you can download it from here -> https://imagej.net/Fiji/Downloads

## Install Windows
First download the JAR file from [latest release (6.10.1)](https://github.com/Jetraw/Bio-Formats/releases/download/22.08.31.1/formats-bsd-6.10.1.jar), or browse [previous releases](https://github.com/Jetraw/Bio-Formats/releases). In the **Release section** you will find the JAR files for **versions**: 6.5.1, 6.6.0, 6.6.1, 6.7.0, 6.8.0, 6.8.1, 6.9.0, 6.9.1, 6.10.0 and 6.10.1.  

Choose the JAR file corresponding to your installed Bio-Formats version and **replace the .jar file** *"formats-bsd-6.x.y.jar"* in the following folder:
*path_to_fiji_app/jars/bio-formats/*.

## Install Linux
Follow the same steps as in the Install Windows section.

Once the .jar file is correctly replaced, an extra step is necessary. 

You need to **add to the LD_LIBRARY_PATH** variable the location of jetraw libraries, then Fiji will be able to find them. Open a terminal and write the following command:  

```
export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/path_to_jetraw_folder/lib/
```

It is recommended to **add this instruction in your own bashrc (/home/user/.bashrc)** file, then everytime a bash environment is generated everything will be correctly set up. **Important to remember** that you will need to **launch Fiji** directly **from a Terminal**. If not the enviroment will not be correctly configured and Jetraw libraries will not be found. 

## Install macOS
Follow the same steps as in the Install Windows section.

Once the .jar file is correctly replaced, an extra step is necessary just in the case that you have not located the **Jetraw UI.app** in the **Applications folder**. 
If you are using a custom folder for Jetraw's installation, you need to configure the DYLD_FALLBACK_LIBRARY_PATH variable to point to your dpcore and jetraw libraries location. 

```
export DYLD_FALLBACK_LIBRARY_PATH=$DYLD_LIBRARY_PATH:/path_to_jetraw_folder/lib/
```

It is recommended to **add this instruction in your bashrc or zshrc (/home/user/.bashrc or /home/user/.zshrc)** file, then everytime a bash/zsh environment is created everything is set up to use the Jetraw codec in Bio-Formats. **Important to remember** that you will need to **launch Fiji** directly **from a Terminal**. If not the enviroment will not be correctly configured and Jetraw libraries will not be found. 

## Usage
Once the installation process is done, you can simply drag and drop a Jetraw compressed TIFF file into Fiji's UI. The application will automatically 
detect that it is a Jetraw compressed image and the Bio-Formats dialog will pop-up offering you different displaying options. 

## Contact
Feel free to use the [issues section](https://github.com/Jetraw/Bio-Formats/issues) to report bugs or request new features. You can also ask questions and give comments by visiting the [discussions](https://github.com/Jetraw/Bio-Formats/discussions), or following the contact information at https://jetraw.com.
