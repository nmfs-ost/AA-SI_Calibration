# Standardized Calibration File

- [1. Property `Standardized Calibration File > file_creation_date`](#file_creation_date)
- [2. Property `Standardized Calibration File > cruise_id`](#cruise_id)
- [3. Property `Standardized Calibration File > calibration_report_title`](#calibration_report_title)
- [4. Property `Standardized Calibration File > calibration_report_DOI`](#calibration_report_DOI)
- [5. Property `Standardized Calibration File > calibration_report`](#calibration_report)
- [6. Property `Standardized Calibration File > channels`](#channels)
  - [6.1. Standardized Calibration File > channels > channelBlock](#channels_items)
    - [6.1.1. Property `Standardized Calibration File > channels > channels items > sonar_serial_number`](#channels_items_sonar_serial_number)
    - [6.1.2. Property `Standardized Calibration File > channels > channels items > sonar_software_version`](#channels_items_sonar_software_version)
    - [6.1.3. Property `Standardized Calibration File > channels > channels items > sonar_software_name`](#channels_items_sonar_software_name)
    - [6.1.4. Property `Standardized Calibration File > channels > channels items > channel`](#channels_items_channel)
    - [6.1.5. Property `Standardized Calibration File > channels > channels items > source_filenames`](#channels_items_source_filenames)
      - [6.1.5.1. Standardized Calibration File > channels > channels items > source_filenames > source_filenames items](#channels_items_source_filenames_items)
    - [6.1.6. Property `Standardized Calibration File > channels > channels items > source_file_type`](#channels_items_source_file_type)
    - [6.1.7. Property `Standardized Calibration File > channels > channels items > source_file_location`](#channels_items_source_file_location)
    - [6.1.8. Property `Standardized Calibration File > channels > channels items > source_file_paths`](#channels_items_source_file_paths)
      - [6.1.8.1. Standardized Calibration File > channels > channels items > source_file_paths > source_file_paths items](#channels_items_source_file_paths_items)
    - [6.1.9. Property `Standardized Calibration File > channels > channels items > frequency`](#channels_items_frequency)
    - [6.1.10. Property `Standardized Calibration File > channels > channels items > absorption_indicative`](#channels_items_absorption_indicative)
    - [6.1.11. Property `Standardized Calibration File > channels > channels items > sound_speed_indicative`](#channels_items_sound_speed_indicative)
    - [6.1.12. Property `Standardized Calibration File > channels > channels items > gain_correction`](#channels_items_gain_correction)
    - [6.1.13. Property `Standardized Calibration File > channels > channels items > sa_correction`](#channels_items_sa_correction)
    - [6.1.14. Property `Standardized Calibration File > channels > channels items > equivalent_beam_angle`](#channels_items_equivalent_beam_angle)
    - [6.1.15. Property `Standardized Calibration File > channels > channels items > beamwidth_transmit_major`](#channels_items_beamwidth_transmit_major)
    - [6.1.16. Property `Standardized Calibration File > channels > channels items > beamwidth_receive_major`](#channels_items_beamwidth_receive_major)
    - [6.1.17. Property `Standardized Calibration File > channels > channels items > beamwidth_transmit_minor`](#channels_items_beamwidth_transmit_minor)
    - [6.1.18. Property `Standardized Calibration File > channels > channels items > beamwidth_receive_minor`](#channels_items_beamwidth_receive_minor)
    - [6.1.19. Property `Standardized Calibration File > channels > channels items > echoangle_major`](#channels_items_echoangle_major)
    - [6.1.20. Property `Standardized Calibration File > channels > channels items > echoangle_minor`](#channels_items_echoangle_minor)
    - [6.1.21. Property `Standardized Calibration File > channels > channels items > echoangle_major_sensitivity`](#channels_items_echoangle_major_sensitivity)
    - [6.1.22. Property `Standardized Calibration File > channels > channels items > echoangle_minor_sensitivity`](#channels_items_echoangle_minor_sensitivity)
    - [6.1.23. Property `Standardized Calibration File > channels > channels items > sample_interval`](#channels_items_sample_interval)
    - [6.1.24. Property `Standardized Calibration File > channels > channels items > transmit_bandwidth`](#channels_items_transmit_bandwidth)
    - [6.1.25. Property `Standardized Calibration File > channels > channels items > transmit_power`](#channels_items_transmit_power)
    - [6.1.26. Property `Standardized Calibration File > channels > channels items > transmit_duration_nominal`](#channels_items_transmit_duration_nominal)
    - [6.1.27. Property `Standardized Calibration File > channels > channels items > calibration_date`](#channels_items_calibration_date)
    - [6.1.28. Property `Standardized Calibration File > channels > channels items > calibration_comments`](#channels_items_calibration_comments)
    - [6.1.29. Property `Standardized Calibration File > channels > channels items > calibration_version`](#channels_items_calibration_version)
    - [6.1.30. Property `Standardized Calibration File > channels > channels items > beam_type`](#channels_items_beam_type)
    - [6.1.31. Property `Standardized Calibration File > channels > channels items > calibration_acquisition_method`](#channels_items_calibration_acquisition_method)
    - [6.1.32. Property `Standardized Calibration File > channels > channels items > sphere_diameter`](#channels_items_sphere_diameter)
    - [6.1.33. Property `Standardized Calibration File > channels > channels items > sphere_material`](#channels_items_sphere_material)
    - [6.1.34. Property `Standardized Calibration File > channels > channels items > temperature`](#channels_items_temperature)
    - [6.1.35. Property `Standardized Calibration File > channels > channels items > salinity`](#channels_items_salinity)

**Title:** Standardized Calibration File

|                           |             |
| ------------------------- | ----------- |
| **Type**                  | `object`    |
| **Required**              | No          |
| **Additional properties** | Not allowed |

**Description:** Schema for a standardized sonar calibration file. Note that many parameter definitions follow the SONAR-netCDF4 convention for sonar data (v2.0, ICES WGFAST Open Data subgroup, generated 2025-02-22 03:11:38 UTC). See https://htmlpreview.github.io/?https://github.com/ices-publications/SONAR-netCDF4/blob/master/Formatted_docs/crr341.html for the full reference.

**Example:**

```json
{
    "file_creation_date": "2025-12-10T18:05:48.252383+00:00",
    "cruise_id": "HB1603",
    "calibration_report_title": null,
    "calibration_report_DOI": null,
    "calibration_report": null,
    "channels": [
        {
            "channel": "GPT  18 kHz 009072056b0e 2-1 ES18-11",
            "source_filenames": [
                "HBB_018kHz_18July2016.cal"
            ],
            "source_file_type": ".cal",
            "source_file_location": null,
            "source_file_paths": null,
            "sonar_serial_number": "009072056b0e",
            "sonar_software_version": "2.4.3",
            "sonar_software_name": null,
            "frequency": 18000.0,
            "absorption_indicative": 0.0018,
            "sound_speed_indicative": 1522.6,
            "gain_correction": 23.08,
            "sa_correction": -0.76,
            "equivalent_beam_angle": -17.0,
            "beamwidth_transmit_major": 11.06,
            "beamwidth_receive_major": 11.06,
            "beamwidth_transmit_minor": 10.56,
            "beamwidth_receive_minor": 10.56,
            "echoangle_major": 0.01,
            "echoangle_minor": -0.07,
            "echoangle_major_sensitivity": 13.9,
            "echoangle_minor_sensitivity": 13.9,
            "sample_interval": 0.000128,
            "transmit_bandwidth": 1570.0,
            "transmit_power": 1000.0,
            "transmit_duration_nominal": 0.001024,
            "calibration_date": "7/18/2016",
            "calibration_comments": "HB Bigelow 18 kHz calibration, 38.1-mm WC sphere, Newport naval anchorage south of bridge, 18 July 2016",
            "calibration_version": null,
            "beam_type": null,
            "calibration_acquisition_method": null,
            "sphere_diameter": null,
            "sphere_material": null,
            "temperature": null,
            "salinity": null
        }
    ]
}
```

| Property                                                 | Pattern | Type           | Deprecated | Definition | Title/Description                                                                                         |
| -------------------------------------------------------- | ------- | -------------- | ---------- | ---------- | --------------------------------------------------------------------------------------------------------- |
| + [file_creation_date](#file_creation_date )             | No      | string         | No         | -          | File creation timestamp                                                                                   |
| - [cruise_id](#cruise_id )                               | No      | string or null | No         | -          | Identifier of the cruise or mission associated with this calibration dataset.                             |
| - [calibration_report_title](#calibration_report_title ) | No      | string or null | No         | -          | Title of the calibration report or document.                                                              |
| - [calibration_report_DOI](#calibration_report_DOI )     | No      | string or null | No         | -          | Digital Object Identifier for the calibration report.                                                     |
| - [calibration_report](#calibration_report )             | No      | string or null | No         | -          | URL or reference to the full calibration report.                                                          |
| + [channels](#channels )                                 | No      | array          | No         | -          | Ordered list of channel parameter blocks sorted by increasing frequency.<br /><br />Collection size: >= 1 |

## <a name="file_creation_date"></a>1. Property `Standardized Calibration File > file_creation_date`

**Title:** File creation timestamp

|              |             |
| ------------ | ----------- |
| **Type**     | `string`    |
| **Required** | Yes         |
| **Format**   | `date-time` |

**Description:** ISO8601 timestamp indicating when this standardized calibration file was produced.

**Example:**

```json
"2025-12-03T20:01:06.089757+00:00"
```

## <a name="cruise_id"></a>2. Property `Standardized Calibration File > cruise_id`

|              |                  |
| ------------ | ---------------- |
| **Type**     | `string or null` |
| **Required** | No               |

**Description:** Identifier of the cruise or mission associated with this calibration dataset.

**Example:**

```json
"HB1603"
```

## <a name="calibration_report_title"></a>3. Property `Standardized Calibration File > calibration_report_title`

|              |                  |
| ------------ | ---------------- |
| **Type**     | `string or null` |
| **Required** | No               |

**Description:** Title of the calibration report or document.

## <a name="calibration_report_DOI"></a>4. Property `Standardized Calibration File > calibration_report_DOI`

|              |                  |
| ------------ | ---------------- |
| **Type**     | `string or null` |
| **Required** | No               |

**Description:** Digital Object Identifier for the calibration report.

## <a name="calibration_report"></a>5. Property `Standardized Calibration File > calibration_report`

|              |                  |
| ------------ | ---------------- |
| **Type**     | `string or null` |
| **Required** | No               |

**Description:** URL or reference to the full calibration report.

## <a name="channels"></a>6. Property `Standardized Calibration File > channels`

|              |         |
| ------------ | ------- |
| **Type**     | `array` |
| **Required** | Yes     |

**Description:** Ordered list of channel parameter blocks sorted by increasing frequency.

Collection size: >= 1

|                      | Array restrictions |
| -------------------- | ------------------ |
| **Min items**        | 1                  |
| **Max items**        | N/A                |
| **Items unicity**    | False              |
| **Additional items** | False              |
| **Tuple validation** | See below          |

| Each item of this array must be | Description                                        |
| ------------------------------- | -------------------------------------------------- |
| [channelBlock](#channels_items) | Calibration parameters for a single sonar channel. |

### <a name="channels_items"></a>6.1. Standardized Calibration File > channels > channelBlock

|                           |                      |
| ------------------------- | -------------------- |
| **Type**                  | `object`             |
| **Required**              | No                   |
| **Additional properties** | Not allowed          |
| **Defined in**            | #/$defs/channelBlock |

**Description:** Calibration parameters for a single sonar channel.

| Property                                                                            | Pattern | Type                    | Deprecated | Definition | Title/Description                                       |
| ----------------------------------------------------------------------------------- | ------- | ----------------------- | ---------- | ---------- | ------------------------------------------------------- |
| - [sonar_serial_number](#channels_items_sonar_serial_number )                       | No      | string or null          | No         | -          | Sonar serial number                                     |
| - [sonar_software_version](#channels_items_sonar_software_version )                 | No      | string or null          | No         | -          | Sonar software version                                  |
| - [sonar_software_name](#channels_items_sonar_software_name )                       | No      | string or null          | No         | -          | Sonar software name                                     |
| + [channel](#channels_items_channel )                                               | No      | string                  | No         | -          | Channel identifier                                      |
| - [source_filenames](#channels_items_source_filenames )                             | No      | array of string or null | No         | -          | Channel source filenames                                |
| - [source_file_type](#channels_items_source_file_type )                             | No      | string or null          | No         | -          | Channel source file type                                |
| - [source_file_location](#channels_items_source_file_location )                     | No      | string or null          | No         | -          | Channel source file location                            |
| - [source_file_paths](#channels_items_source_file_paths )                           | No      | array of string or null | No         | -          | Channel source file paths                               |
| + [frequency](#channels_items_frequency )                                           | No      | number                  | No         | -          | Acoustic frequency                                      |
| - [absorption_indicative](#channels_items_absorption_indicative )                   | No      | number                  | No         | -          | Indicative acoustic absorption                          |
| - [sound_speed_indicative](#channels_items_sound_speed_indicative )                 | No      | number                  | No         | -          | Indicative sound speed                                  |
| - [gain_correction](#channels_items_gain_correction )                               | No      | number                  | No         | -          | Gain correction                                         |
| - [sa_correction](#channels_items_sa_correction )                                   | No      | number                  | No         | -          | Sa correction                                           |
| - [equivalent_beam_angle](#channels_items_equivalent_beam_angle )                   | No      | number                  | No         | -          | Equivalent beam angle                                   |
| - [beamwidth_transmit_major](#channels_items_beamwidth_transmit_major )             | No      | number                  | No         | -          | Half power one-way transmit beam width along major axis |
| - [beamwidth_receive_major](#channels_items_beamwidth_receive_major )               | No      | number                  | No         | -          | Half power one-way receive beam width along major axis  |
| - [beamwidth_transmit_minor](#channels_items_beamwidth_transmit_minor )             | No      | number                  | No         | -          | Half power one-way transmit beam width along minor axis |
| - [beamwidth_receive_minor](#channels_items_beamwidth_receive_minor )               | No      | number                  | No         | -          | Half power one-way receive beam width along minor axis  |
| - [echoangle_major](#channels_items_echoangle_major )                               | No      | number                  | No         | -          | Echo arrival angle in the major beam coordinate         |
| - [echoangle_minor](#channels_items_echoangle_minor )                               | No      | number                  | No         | -          | Echo arrival angle in the minor beam coordinate         |
| - [echoangle_major_sensitivity](#channels_items_echoangle_major_sensitivity )       | No      | number                  | No         | -          | Major angle scaling factor                              |
| - [echoangle_minor_sensitivity](#channels_items_echoangle_minor_sensitivity )       | No      | number                  | No         | -          | Minor angle scaling factor                              |
| - [sample_interval](#channels_items_sample_interval )                               | No      | number                  | No         | -          | Interval between recorded raw data samples              |
| - [transmit_bandwidth](#channels_items_transmit_bandwidth )                         | No      | number                  | No         | -          | Nominal bandwidth of transmitted pulse                  |
| - [transmit_power](#channels_items_transmit_power )                                 | No      | number                  | No         | -          | Nominal transmit power                                  |
| - [transmit_duration_nominal](#channels_items_transmit_duration_nominal )           | No      | number                  | No         | -          | Nominal duration of transmitted pulse                   |
| - [calibration_date](#channels_items_calibration_date )                             | No      | string or null          | No         | -          | Calibration date                                        |
| - [calibration_comments](#channels_items_calibration_comments )                     | No      | string or null          | No         | -          | Calibration comments                                    |
| - [calibration_version](#channels_items_calibration_version )                       | No      | string or null          | No         | -          | Calibration processing version                          |
| - [beam_type](#channels_items_beam_type )                                           | No      | string or null          | No         | -          | Transducer beam type                                    |
| - [calibration_acquisition_method](#channels_items_calibration_acquisition_method ) | No      | string or null          | No         | -          | Calibration acquisition method                          |
| - [sphere_diameter](#channels_items_sphere_diameter )                               | No      | number or null          | No         | -          | Calibration sphere diameter                             |
| - [sphere_material](#channels_items_sphere_material )                               | No      | string or null          | No         | -          | Calibration sphere material                             |
| - [temperature](#channels_items_temperature )                                       | No      | number or null          | No         | -          | Water temperature                                       |
| - [salinity](#channels_items_salinity )                                             | No      | number or null          | No         | -          | Water salinity                                          |

#### <a name="channels_items_sonar_serial_number"></a>6.1.1. Property `Standardized Calibration File > channels > channels items > sonar_serial_number`

**Title:** Sonar serial number

|              |                  |
| ------------ | ---------------- |
| **Type**     | `string or null` |
| **Required** | No               |

**Description:** Manufacturer serial number for the sonar head associated with this channel.

Reference: SONAR-netCDF4 2.0 Sonar.sonar_serial_number

#### <a name="channels_items_sonar_software_version"></a>6.1.2. Property `Standardized Calibration File > channels > channels items > sonar_software_version`

**Title:** Sonar software version

|              |                  |
| ------------ | ---------------- |
| **Type**     | `string or null` |
| **Required** | No               |

**Description:** Version string of the sonar software controlling this channel.

Reference: SONAR-netCDF4 2.0 Sonar.sonar_software_version

**Example:**

```json
"2.4.3"
```

#### <a name="channels_items_sonar_software_name"></a>6.1.3. Property `Standardized Calibration File > channels > channels items > sonar_software_name`

**Title:** Sonar software name

|              |                  |
| ------------ | ---------------- |
| **Type**     | `string or null` |
| **Required** | No               |

**Description:** Name of the sonar control or acquisition software.

Reference: SONAR-netCDF4 2.0 Sonar.sonar_software_name

#### <a name="channels_items_channel"></a>6.1.4. Property `Standardized Calibration File > channels > channels items > channel`

**Title:** Channel identifier

|              |          |
| ------------ | -------- |
| **Type**     | `string` |
| **Required** | Yes      |

**Description:** Identifier of the transceiver/channel.

#### <a name="channels_items_source_filenames"></a>6.1.5. Property `Standardized Calibration File > channels > channels items > source_filenames`

**Title:** Channel source filenames

|              |                           |
| ------------ | ------------------------- |
| **Type**     | `array of string or null` |
| **Required** | No                        |

**Description:** List of calibration source files that produced this channel's parameters.

**Example:**

```json
[
    "HBB_018kHz_18July2016.cal"
]
```

|                      | Array restrictions |
| -------------------- | ------------------ |
| **Min items**        | N/A                |
| **Max items**        | N/A                |
| **Items unicity**    | False              |
| **Additional items** | False              |
| **Tuple validation** | See below          |

| Each item of this array must be                                  | Description |
| ---------------------------------------------------------------- | ----------- |
| [source_filenames items](#channels_items_source_filenames_items) | -           |

##### <a name="channels_items_source_filenames_items"></a>6.1.5.1. Standardized Calibration File > channels > channels items > source_filenames > source_filenames items

|              |          |
| ------------ | -------- |
| **Type**     | `string` |
| **Required** | No       |

#### <a name="channels_items_source_file_type"></a>6.1.6. Property `Standardized Calibration File > channels > channels items > source_file_type`

**Title:** Channel source file type

|              |                  |
| ------------ | ---------------- |
| **Type**     | `string or null` |
| **Required** | No               |

**Description:** File extension or descriptor describing the calibration source files linked to this channel.

**Examples:**

```json
".raw"
```

```json
".cal"
```

#### <a name="channels_items_source_file_location"></a>6.1.7. Property `Standardized Calibration File > channels > channels items > source_file_location`

**Title:** Channel source file location

|              |                  |
| ------------ | ---------------- |
| **Type**     | `string or null` |
| **Required** | No               |

**Description:** Human-readable location of the calibration source files that contributed to this channel.

**Examples:**

```json
"NCEI"
```

```json
"OMAO"
```

```json
"HDD"
```

#### <a name="channels_items_source_file_paths"></a>6.1.8. Property `Standardized Calibration File > channels > channels items > source_file_paths`

**Title:** Channel source file paths

|              |                           |
| ------------ | ------------------------- |
| **Type**     | `array of string or null` |
| **Required** | No                        |

**Description:** Absolute or relative paths to the calibration source files for this channel.

|                      | Array restrictions |
| -------------------- | ------------------ |
| **Min items**        | N/A                |
| **Max items**        | N/A                |
| **Items unicity**    | False              |
| **Additional items** | False              |
| **Tuple validation** | See below          |

| Each item of this array must be                                    | Description |
| ------------------------------------------------------------------ | ----------- |
| [source_file_paths items](#channels_items_source_file_paths_items) | -           |

##### <a name="channels_items_source_file_paths_items"></a>6.1.8.1. Standardized Calibration File > channels > channels items > source_file_paths > source_file_paths items

|              |          |
| ------------ | -------- |
| **Type**     | `string` |
| **Required** | No       |

#### <a name="channels_items_frequency"></a>6.1.9. Property `Standardized Calibration File > channels > channels items > frequency`

**Title:** Acoustic frequency

|              |          |
| ------------ | -------- |
| **Type**     | `number` |
| **Required** | Yes      |

**Description:** Frequency of the receive echo from spectral analysis of the FM pulse or frequency of the CW pulse.

Precision: 10

Reference: SONAR-netCDF4 2.0 Sonar/Beam_group.frequency

Units: Hz

Numeric constraints: >= 0.0

**Examples:**

```json
18000.0
```

```json
38000.0
```

```json
70000.0
```

#### <a name="channels_items_absorption_indicative"></a>6.1.10. Property `Standardized Calibration File > channels > channels items > absorption_indicative`

**Title:** Indicative acoustic absorption

|              |          |
| ------------ | -------- |
| **Type**     | `number` |
| **Required** | No       |

**Description:** Indicative absorption values used to calculate the time-varied gain (TVG) in the absence of detailed data.

Precision: 10

Reference: SONAR-netCDF4 2.0 Environment.absorption_indicative

Units: dB/m

Numeric constraints: >= 0.0

**Examples:**

```json
0.01
```

```json
0.02
```

#### <a name="channels_items_sound_speed_indicative"></a>6.1.11. Property `Standardized Calibration File > channels > channels items > sound_speed_indicative`

**Title:** Indicative sound speed

|              |          |
| ------------ | -------- |
| **Type**     | `number` |
| **Required** | No       |

**Description:** Mean sound speed in water used to calculate echo range when detailed profiles are unavailable.

Precision: 2

Reference: SONAR-netCDF4 2.0 Environment.sound_speed_indicative

Units: m/s

Numeric constraints: >= 0.0

**Example:**

```json
1522.6
```

#### <a name="channels_items_gain_correction"></a>6.1.12. Property `Standardized Calibration File > channels > channels items > gain_correction`

**Title:** Gain correction

|              |          |
| ------------ | -------- |
| **Type**     | `number` |
| **Required** | No       |

**Description:** Gain correction set from a calibration exercise (required for type 2 conversion equations).

Precision: 2

Reference: SONAR-netCDF4 2.0 Sonar/Beam_group.gain_correction

Units: dB

**Examples:**

```json
24.06
```

```json
25.41
```

#### <a name="channels_items_sa_correction"></a>6.1.13. Property `Standardized Calibration File > channels > channels items > sa_correction`

**Title:** Sa correction

|              |          |
| ------------ | -------- |
| **Type**     | `number` |
| **Required** | No       |

**Description:** Nautical area scattering coefficient correction derived from calibration.

Precision: 2

Units: dB

**Examples:**

```json
-0.68
```

```json
-0.32
```

#### <a name="channels_items_equivalent_beam_angle"></a>6.1.14. Property `Standardized Calibration File > channels > channels items > equivalent_beam_angle`

**Title:** Equivalent beam angle

|              |          |
| ------------ | -------- |
| **Type**     | `number` |
| **Required** | No       |

**Description:** Equivalent beam angle of the receive beam.

Precision: 2

Reference: SONAR-netCDF4 2.0 Sonar/Beam_group.equivalent_beam_angle

Units: dB re sr

**Example:**

```json
-17.0
```

#### <a name="channels_items_beamwidth_transmit_major"></a>6.1.15. Property `Standardized Calibration File > channels > channels items > beamwidth_transmit_major`

**Title:** Half power one-way transmit beam width along major axis

|              |          |
| ------------ | -------- |
| **Type**     | `number` |
| **Required** | No       |

**Description:** One-way beam width at half-power down in the horizontal (major) direction of the transmit beam.

Precision: 2

Reference: SONAR-netCDF4 2.0 Sonar/Beam_group.beamwidth_transmit_major

Units: arc_degree

Numeric constraints: >= 0.0, <= 360.0

**Examples:**

```json
11.06
```

```json
6.97
```

#### <a name="channels_items_beamwidth_receive_major"></a>6.1.16. Property `Standardized Calibration File > channels > channels items > beamwidth_receive_major`

**Title:** Half power one-way receive beam width along major axis

|              |          |
| ------------ | -------- |
| **Type**     | `number` |
| **Required** | No       |

**Description:** One-way beam width at half-power down in the horizontal (major) direction of the receive beam.

Precision: 2

Reference: SONAR-netCDF4 2.0 Sonar/Beam_group.beamwidth_receive_major

Units: arc_degree

Numeric constraints: >= 0.0, <= 360.0

**Examples:**

```json
11.06
```

```json
6.97
```

#### <a name="channels_items_beamwidth_transmit_minor"></a>6.1.17. Property `Standardized Calibration File > channels > channels items > beamwidth_transmit_minor`

**Title:** Half power one-way transmit beam width along minor axis

|              |          |
| ------------ | -------- |
| **Type**     | `number` |
| **Required** | No       |

**Description:** One-way beam width at half-power down in the vertical (minor) direction of the transmit beam.

Precision: 2

Reference: SONAR-netCDF4 2.0 Sonar/Beam_group.beamwidth_transmit_minor

Units: arc_degree

Numeric constraints: >= 0.0, <= 360.0

**Examples:**

```json
10.56
```

```json
6.87
```

#### <a name="channels_items_beamwidth_receive_minor"></a>6.1.18. Property `Standardized Calibration File > channels > channels items > beamwidth_receive_minor`

**Title:** Half power one-way receive beam width along minor axis

|              |          |
| ------------ | -------- |
| **Type**     | `number` |
| **Required** | No       |

**Description:** One-way beam width at half-power down in the vertical (minor) direction of the receive beam.

Precision: 2

Reference: SONAR-netCDF4 2.0 Sonar/Beam_group.beamwidth_receive_minor

Units: arc_degree

Numeric constraints: >= 0.0, <= 360.0

**Examples:**

```json
10.56
```

```json
6.87
```

#### <a name="channels_items_echoangle_major"></a>6.1.19. Property `Standardized Calibration File > channels > channels items > echoangle_major`

**Title:** Echo arrival angle in the major beam coordinate

|              |          |
| ------------ | -------- |
| **Type**     | `number` |
| **Required** | No       |

**Description:** Electrical phase-derived arrival angle relative to the major beam coordinate.

Precision: 2

Reference: SONAR-netCDF4 2.0 Sonar/Beam_group.echoangle_major

Units: arc_degree

Numeric constraints: >= -180.0, <= 180.0

**Examples:**

```json
0.01
```

```json
-0.12
```

#### <a name="channels_items_echoangle_minor"></a>6.1.20. Property `Standardized Calibration File > channels > channels items > echoangle_minor`

**Title:** Echo arrival angle in the minor beam coordinate

|              |          |
| ------------ | -------- |
| **Type**     | `number` |
| **Required** | No       |

**Description:** Electrical phase-derived arrival angle relative to the minor beam coordinate.

Precision: 2

Reference: SONAR-netCDF4 2.0 Sonar/Beam_group.echoangle_minor

Units: arc_degree

Numeric constraints: >= -180.0, <= 180.0

**Examples:**

```json
-0.07
```

```json
-0.09
```

#### <a name="channels_items_echoangle_major_sensitivity"></a>6.1.21. Property `Standardized Calibration File > channels > channels items > echoangle_major_sensitivity`

**Title:** Major angle scaling factor

|              |          |
| ------------ | -------- |
| **Type**     | `number` |
| **Required** | No       |

**Description:** Scaling factor converting electrical phase differences to physical echo arrival angles (major axis).

Precision: 10

Reference: SONAR-netCDF4 2.0 Sonar/Beam_group.echoangle_major_sensitivity

Units: 1

Numeric constraints: >= 0.0

**Examples:**

```json
13.9
```

```json
23.0
```

#### <a name="channels_items_echoangle_minor_sensitivity"></a>6.1.22. Property `Standardized Calibration File > channels > channels items > echoangle_minor_sensitivity`

**Title:** Minor angle scaling factor

|              |          |
| ------------ | -------- |
| **Type**     | `number` |
| **Required** | No       |

**Description:** Scaling factor converting electrical phase differences to physical echo arrival angles (minor axis).

Precision: 10

Reference: SONAR-netCDF4 2.0 Sonar/Beam_group.echoangle_minor_sensitivity

Units: 1

Numeric constraints: >= 0.0

**Examples:**

```json
13.9
```

```json
23.0
```

#### <a name="channels_items_sample_interval"></a>6.1.23. Property `Standardized Calibration File > channels > channels items > sample_interval`

**Title:** Interval between recorded raw data samples

|              |          |
| ------------ | -------- |
| **Type**     | `number` |
| **Required** | No       |

**Description:** Time between individual samples along a beam (common for all beams in a ping).

Precision: 6

Reference: SONAR-netCDF4 2.0 Sonar/Beam_group.sample_interval

Units: s

Numeric constraints: >= 0.0

**Example:**

```json
0.000128
```

#### <a name="channels_items_transmit_bandwidth"></a>6.1.24. Property `Standardized Calibration File > channels > channels items > transmit_bandwidth`

**Title:** Nominal bandwidth of transmitted pulse

|              |          |
| ------------ | -------- |
| **Type**     | `number` |
| **Required** | No       |

**Description:** Estimated bandwidth of the transmitted pulse.

Precision: 10

Reference: SONAR-netCDF4 2.0 Sonar/Beam_group.transmit_bandwidth

Units: Hz

Numeric constraints: >= 0.0

**Examples:**

```json
1570.0
```

```json
3030.0
```

#### <a name="channels_items_transmit_power"></a>6.1.25. Property `Standardized Calibration File > channels > channels items > transmit_power`

**Title:** Nominal transmit power

|              |          |
| ------------ | -------- |
| **Type**     | `number` |
| **Required** | No       |

**Description:** Electrical transmit power used for the ping (required for type 1 conversion equations).

Precision: 10

Reference: SONAR-netCDF4 2.0 Sonar/Beam_group.transmit_power

Units: W

Numeric constraints: >= 0.0

**Examples:**

```json
1000.0
```

```json
300.0
```

#### <a name="channels_items_transmit_duration_nominal"></a>6.1.26. Property `Standardized Calibration File > channels > channels items > transmit_duration_nominal`

**Title:** Nominal duration of transmitted pulse

|              |          |
| ------------ | -------- |
| **Type**     | `number` |
| **Required** | No       |

**Description:** Duration of the transmitted pulse prior to reception (not the effective duration).

Precision: 6

Reference: SONAR-netCDF4 2.0 Sonar/Beam_group.transmit_duration_nominal

Units: s

Numeric constraints: >= 0.0

**Example:**

```json
0.001024
```

#### <a name="channels_items_calibration_date"></a>6.1.27. Property `Standardized Calibration File > channels > channels items > calibration_date`

**Title:** Calibration date

|              |                  |
| ------------ | ---------------- |
| **Type**     | `string or null` |
| **Required** | No               |

**Description:** Date associated with the calibration measurements. Derived from calibration report files, so format is free-form.

**Example:**

```json
"7/18/2016"
```

#### <a name="channels_items_calibration_comments"></a>6.1.28. Property `Standardized Calibration File > channels > channels items > calibration_comments`

**Title:** Calibration comments

|              |                  |
| ------------ | ---------------- |
| **Type**     | `string or null` |
| **Required** | No               |

**Description:** Narrative notes captured during the calibration event.

#### <a name="channels_items_calibration_version"></a>6.1.29. Property `Standardized Calibration File > channels > channels items > calibration_version`

**Title:** Calibration processing version

|              |                  |
| ------------ | ---------------- |
| **Type**     | `string or null` |
| **Required** | No               |

**Description:** Software or procedure version used when producing these calibration parameters. *add specifics

#### <a name="channels_items_beam_type"></a>6.1.30. Property `Standardized Calibration File > channels > channels items > beam_type`

**Title:** Transducer beam type

|              |                  |
| ------------ | ---------------- |
| **Type**     | `string or null` |
| **Required** | No               |

**Description:** Describes the physical beam type of the transducer (e.g., split-beam, single).

Reference: SONAR-netCDF4 2.0 Sonar/Beam_group.beam_type

#### <a name="channels_items_calibration_acquisition_method"></a>6.1.31. Property `Standardized Calibration File > channels > channels items > calibration_acquisition_method`

**Title:** Calibration acquisition method

|              |                  |
| ------------ | ---------------- |
| **Type**     | `string or null` |
| **Required** | No               |

**Description:** Brief description of the calibration workflow or platform used.

#### <a name="channels_items_sphere_diameter"></a>6.1.32. Property `Standardized Calibration File > channels > channels items > sphere_diameter`

**Title:** Calibration sphere diameter

|              |                  |
| ------------ | ---------------- |
| **Type**     | `number or null` |
| **Required** | No               |

**Description:** Diameter of the calibration sphere.

Precision: 10

Units: mm

Numeric constraints: >= 0.0

#### <a name="channels_items_sphere_material"></a>6.1.33. Property `Standardized Calibration File > channels > channels items > sphere_material`

**Title:** Calibration sphere material

|              |                  |
| ------------ | ---------------- |
| **Type**     | `string or null` |
| **Required** | No               |

**Description:** Material of the calibration sphere.

**Example:**

```json
"tungsten carbide"
```

#### <a name="channels_items_temperature"></a>6.1.34. Property `Standardized Calibration File > channels > channels items > temperature`

**Title:** Water temperature

|              |                  |
| ------------ | ---------------- |
| **Type**     | `number or null` |
| **Required** | No               |

**Description:** Ambient water temperature recorded during calibration.

Precision: 2

Units: degC

#### <a name="channels_items_salinity"></a>6.1.35. Property `Standardized Calibration File > channels > channels items > salinity`

**Title:** Water salinity

|              |                  |
| ------------ | ---------------- |
| **Type**     | `number or null` |
| **Required** | No               |

**Description:** Water salinity during calibration.

Precision: 10

Units: psu

Numeric constraints: >= 0.0

----------------------------------------------------------------------------------------------------------------------------
Generated using [json-schema-for-humans](https://github.com/coveooss/json-schema-for-humans) on 2025-12-11 at 12:37:14 -0700