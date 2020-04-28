# Robaux SWT16+

With the [Robaux SWT16+](https://robaux.io/swt16plus) you can now use MIDI devices like drum machines or samplers. Each track of the sequencer can now output an individual MIDI note to one of 16 MIDI channels. The firmware update is not difficult, but the update process is a bit fumbling.

## MIDI Adapter

To enable the Sequencer to output MIDI data, it is necessary to build an adapter. However, this is relatively simple. The following is a diagram of how the adapter is constructed. 

![MIDI Adapter](https://robaux.io/update/swt16plus/swt16plusMIDIAdapter.jpg)

## Update your Module

#### <span style="color:red">Attention: When updating the firmware, all patterns and settings will be overwritten!</span>

To transfer a firmware update you need a computer with a serial USB interface. Since the heart of the sequencer is an ATMega328, especially an [Arduino UNO](https://store.arduino.cc/arduino-uno-rev3) is excellent. But it also work with standard interfaces such as FT232 or similar.

You also need the transfer program [AVRDude](https://typeunsafe.wordpress.com/2011/07/22/programming-arduino-with-avrdude/) which comes with the [Arduino software](https://www.arduino.cc/en/main/software). AVRDude is a command line utility. But there are also graphical interfaces, for example [HexUploader](http://paulkaplan.me/HexUploader/) (MacOS) or [Xloader](http://xloader.russemotto.com/) (Windows).

The [Update](https://github.com/robaux/swt16plusMIDI/tree/master/update) folder contains the firmware hex files which you can transfer to the device.

Select the version you want to transfer. Connect your Robaux SWT16+ to your serial port as shown in the pictures.

Select your serial interface in AVRDude or a corresponding program as well as the HEX file and transfer it to the Robaux SWT16+. If you have any questions, please contact update@robaux.io

---

![Updating using a Arduino Uno](https://robaux.io/update/swt16plus/updatingArduinoUno3.jpg)

---

![Updating using a FT232](https://robaux.io/update/swt16plus/updatingFT232.jpg)
