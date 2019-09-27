# Alorium Web Loader

The Alorium Web Loader is an application that facilitates web-based loading of new FPGA images to your XLR8, Snō or Hinj boards.  

It does this by creating a websocket server and opening port 8989 on the user's computer. Once this port is open, our [Web Loader website](http://rpd.aloriumtech.com/) send commands to the websocket, enabling it to write a new image to a connected Alorium board.

### Credits
This application was created from a fork of the [serial-port-json-server](https://github.com/chilipeppr/serial-port-json-server) by [John Lauer.](https://github.com/chilipeppr)

### *Note: This is a non-SSL connection*
Please note that traffic sent to the websocket between a website and the user's machine is unencrypted.

<hr>

### Usage

There is a separate Alorium Web Loader binary for each supported operating system.  Currently, we only support macOS; however, the Windows application will be available soon.  

**1. Download application**
To get the program, navigate to the folder for your operating system and click on the associated ZIP file. From there, you will be able to download and extract program to your computer. 

**2. Run application**
Change to the directory created after extracting the ZIP file and run the program.  The server application is called *serial-port-json-server*.  You may be prompted by your operating system to allow the application to run.  

**3. Go to the Alorium's Web Loader page**
In a web browser, navigate to the site [rpd.aloriumtech.com](http://rpd.aloriumtech.com/).  

Connect an XLR8, Snō or Hinj board via USB, then click the "Get Serials" button to list the availble serial ports.  Select the serial port connected to your board from the drop-down 

Choose the image you would like to put on the board from the list of available images and click the Burn button.  

It will take some time, and you will see communication LEDs on your board toggling while the image is being written. Once it is finished, you can shut down the Alorium Web Loader application and resume using your board.

