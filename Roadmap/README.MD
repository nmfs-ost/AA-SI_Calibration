# Calibration File Road Map
Apply the correct calibration values to data files.

## Kongsberg
This section describes calibration parameters and files for the Kongsberg (aka Simarad) echosounders: EK500, EK60, and EK80. Other sounders will be added as we acquire data from them.

### EK500
The EK500 stores calibration values in a file that is read by the EK500 echosounder upon startup. The calibration values are not recorded in the data files. TBD


### EK60/ER60
Calibration values for EK60/ER60 data files are written to each data file. These values are not applied to the data (e.g., "power") in the file, but are applied by the processing software after the data have been read into the software. Not applying the calibration values to the data has benefits and limitations.  A benefit is that modifications to the calibration values can be made and applied in software in the event that the embedded values are incorrect. Limitations are that the data are not "calibrated" and can not be used directly by only reading the file, users not accustomed to Kongsberg data may not understand that they need to apply the calibration values to the data prior to analysis, and changes to the calibration values must be tracked throughout the lifecycle of the data file.

#### Channels
EK60/ER60 data files can contain data from multiple echosounders and transducers, and each echosounder can be configured in its own way. Kongsberg identifies each combination of transceiver-transducer pair and operational configuration as a "channel". The channel identification is a character string with space-delimited components that provide information about the configuration.   An example EK60/ER60 channel ID is:
**GPT  18 kHz 009072034d45 1-1 ES18-11**
where the components are:
- "GPT": the transceiver identification. "GPT" is a General Purpose Transceiver (GPT).
  - The only sounder used by the EK60 system.
- "18": the transmitted acoustic frequency.
- "kHz": the units of the transmitted acoustic frequency. 
  - Combining the frequency value and units into one string is a convenient way to express the transmitted acoustic frequency.
- "009072034d45": The serial number of the transceiver, in this case a GPT.
- "1-1": Combination of a channel number and configuration, as defined by Kongsberg. 
  - The channel number is defined by the order in which each transceiver was installed in the ER60 acquisition software. 
  - The configuration is based on the acquisition settings.
  - NEED TO CONFIRM & PROVIDE MORE DETAILS.
- "ES18-11": The transducer model. 
  - This value is obtained from the installation menu, i.e., a transceiver-transducer pair are defined in the installation section of the ER60 acquisition software.

The "channel number - configuration ID" can change based on the installation order of the transceiver-transducer pair and configuration. While this can not change within a file, it can change among files. For example, a transceiver-transducer pair could be installed/reinstalled during a survey in an order that is different from the previous order. In this case, the same calibration values could/should be applied for different channel IDs.

### EK80
Calibration values for EK80 data files are written to each data file. These values are not applied to the data (e.g., "power") in the file, but are applied by the processing software after the data have been read into the software. Not applying the calibration values to the data has benefits and limitations.  A benefit is that modifications to the calibration values can be made and applied in software in the event that the embedded values are incorrect. Limitations are that the data are not "calibrated" and can not be used directly by only reading the file, users not accustomed to Kongsberg data may not understand that they need to apply the calibration values to the data prior to analysis, and changes to the calibration values must be tracked throughout the lifecycle of the data file.

#### Channels
EK80 data files can contain data from multiple echosounders and transducers, and each echosounder can be configured in its own way. Kongsberg identifies each combination of transceiver-transducer pair and operational configuration as a "channel". The channel identification is a character string with space-delimited components that provide information about the configuration.   An example EK80 channel ID is:
**WBT 978217-15 ES38-7_1**
where the components are:
- "WBT": the transceiver identification. "WBT" is a Wide Band Transceiver (WBT). 
  - The EK80 acquisition software can also operate the EK60 General Purpose Transceiver (GPT).
- "978217015": The serial number of the transceiver, in this case a WBT.
- "ES38-7_1": A combination of the transducer model and configuration. 
  - The transducer model value is obtained from the installation menu, i.e., a transceiver-transducer pair are defined in the installation section of the EK80 acquisition software, and also provides the transmit frequency in kHz (e.g., the "38" indicates 38 kHz). 
  - NEED TO CONFIRM & PROVIDE MORE DETAILS.

### Implementation
Overarching Rules:
- Calibration values do not change within a file. 
  - The calibration values written for each channel are constant throughout the file.  
- Calibration values within a file are immutable. 
  - We do not overwrite the values within a file.
- We can modify calibration values for time periods within a data file after the file has been imported to the processing software.
- A channel ID is unique within a data file, but not necessarily among data files.

- Stage 1
  - The user selects a set of data files to:
    1. Upload the files to NCEI, e.g., using Tugboat
    1. Upload the files to the AA-SI storage bucket
    1. Download the files to local storage

- Stage 2
  - The selected data files are read and a list of unique channels is generated.
