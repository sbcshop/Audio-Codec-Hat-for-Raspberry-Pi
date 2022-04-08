# Audio-Codec-Hat-for-Raspberry-Pi

<img src= "https://github.com/sbcshop/Audio-Codec-Hat-for-Raspberry-Pi/blob/main/images/img.JPG" />

### Audio Codec HAT is a low-power, high-quality stereo CODEC designed for portable digital audio applications which are based on WM8960 IC that have the advantages like Low leakage, excellent PSRR, and pop/click suppression mechanisms that allow direct battery connection to the speaker supply. Flexible speaker boost settings allow speaker output power to be maximized while minimizing another analog supply current.

<img src= "https://github.com/sbcshop/Audio-Codec-Hat-for-Raspberry-Pi/blob/main/images/img1.JPG" />

## Installation Process
### steps :
   * Download the repository  ``` git clone https://github.com/sbcshop/Audio-Codec-Hat-for-Raspberry-Pi ```
   * Go to below directory to Install the driver (follow steps)
       * ``` cd Audio-Codec-Hat-for-Raspberry-Pi ```
       * ```sudo chmod 777 *```
       * ``` sudo ./install.sh ```
       * if you face issue like this **sudo: ./install.sh: command not found** Then follow below command
        * ```sudo ./install.sh```
   * After installation reboot raspberry pi  ``` sudo reboot ```
   * Perform the following command to restart the service if the 3.5mm jack has no audio output.  
       * ``` sudo systemctl restart wm8960-soundcard.service ```
       
   * **If you notice a noise problem with the  Audio Codec , reinstall the driver and try it again.**
   
###  Mic Test
Replace   **0**  in  **Dhw:0**  with your card number, command to know card number ``` arecord -l ```

```sudo arecord -f cd -Dhw:0 | aplay -Dhw:0``` 




         
