# google-enrollment
This are the scripts that we use to enroll chromebooks from Rubber Ducky

### Requirements
 * Rubber Ducky
* Computer with text editor
* Chromebook to enroll
* Admin account or with enrollment permissions.

#### Processing time: 
- 2 minutes

### On any computer
* Open the script from Encoder folder.
* Edit the text and replace the SSID and wireless password, account and account password to enroll.
* Compiling the with the Jar or [Web Tool Script]((https://ducktoolkit.com/encoder/)) to a binary file.
* Open the Rubber ducky and save the script in SD card form inside, once saved the script, reclosing the USB.

### On the Chromebook to enroll
* Turn the Chromebook and wait the first screen
* Insert the Rubber ducky and let enrolls alone.
* Once enrolled in the Chromebook, disconnect the Rubber Ducky and turn off the Chromebook.



The Rubber Ducky is a USB device that simulates a keyboard and executes a sequence of keystrokes previously set in a script. The script must change the parameters:

- **_WIFI_SSID_:** wireless SSID
- **WIFI_SSID_Password_network:** network password 
- **EnrollmentEmail@domain.com_:** Email administrator or user with privileges for enrollment:
- **_EnrollmentEmail_Password_email:** password 

### Compile
To compile the binary file just run this from encoder folder: 
```sh
$ java -jar encoder.jar -l resources/us.properties -i script.txt -o inject.bin
```

Where:
- **us.properties** is the config for keyboard (US)
- **script.txt** is input file
- **inject.bin** is outpu file

**OR**
You can use [Web App Compiler](https://ducktoolkit.com/encoder/)
