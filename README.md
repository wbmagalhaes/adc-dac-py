# addapy
Python 3 wrapper for [Waveshare High Precision AD/DA board](https://www.waveshare.com/wiki/High-Precision_AD/DA_Board) (ADS1256 and DAC8532)

## Installing the library
Navigate to the cloned directory on your Raspberry Pi and use the following command to install addapy.
```
sudo python3 setup.py install
```

## Running sample code
The C library requires root permission, so any time you run a script with addapy, you must run it with sudo.
```
sudo python3 example.py
```

## Functions
### start_adda
Start interface and set gain, sampling rate, and scan mode.

### stop_adda
End interface.

### read_adc
Command the chip to collect data.

### get_channel_raw
Read the raw data from a single ADC channel

### get_channel_volts
Read the data converted to voltage from a single ADC channel.

### write_volts
Set the voltage value to a single DAC channel.