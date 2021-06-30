# Jetraw Fiji Bio-Formats
This is the Fiji Bio-Formats plug-in for Jetraw. With this Bio-Formats plug-in version you will be able to read Jetraw compressed TIFF files using your current Fiji installation. For more info visit https://www.jetraw.com/

## Requirements
- **Jetraw installed** on a Windows computer (MacOS and Linux coming soon) and installation folder in PATH.
- **Fiji installed** with Bio-Formats plug-in (accepted versions 6.5.1, 6.6.0 and 6.6.1)
*Note:* if you do not have Fiji installed you can download it from here -> https://imagej.net/Fiji/Downloads

## Installation
First download the JAR file from [latest release (6.6.1)](https://github.com/Jetraw/Bio-Formats/releases/download/21.06.16.1/formats-bsd-6.6.1.jar), or browse [previous releases](https://github.com/Jetraw/Bio-Formats/releases). In the **Release section** you will find the JAR files for **versions**: 6.5.1, 6.6.0 and 6.6.1.  

Choose the JAR file corresponding to your installed Bio-Formats version and **replace the .jar file** *"formats-bsd-6.x.y.jar"* in the following folder:
*path_to_fiji_app/jars/bio-formats/*.

## Usage
Once the installation process is done, you can simply drag and drop a Jetraw compressed TIFF file into Fiji's UI. The application will automatically 
detect that it is a Jetraw compressed image and the Bio-Formats dialog will pop-up offering you different displaying options. 

## Contact
Feel free to use the [issues section](https://github.com/Jetraw/Bio-Formats/issues) to report bugs or request new features. You can also ask questions and give comments by visiting the [discussions](https://github.com/Jetraw/Bio-Formats/discussions), or following the contact information at https://jetraw.com.
