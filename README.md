# Cosmic LoRa Breakout

## List of Acronym
| Acronym    | Stands for |
|------------|-----------------------|
| NC         | Not Connected |
| SPI        | Serial Peripheral Interface |
| MOSI       | Master In Slave Out |
| MISO       | Master Out Slave In |
| SCK        | Serial Clock |
| CIPO       | Controller In, Peripheral Out |
| COPI       | Controller Out Peripheral In |
| SS         | Slave Select |

## Compatability
| Dev Board    | Variant 3.3V | Variant 5V | Variant Dual 3.3V & 5V |
|--------------|-------------|-----------|-----------------------|
| ESP32        | :heavy_check_mark:           | :x:         | :heavy_check_mark:                     |
| ESP8266      | :heavy_check_mark:           | :x:         | :heavy_check_mark:                     |
| Arduino Uno R3  | :x:           | :heavy_check_mark:         | :heavy_check_mark:                     |
| Arduino Mega R3 | :x:           | :heavy_check_mark:         | :heavy_check_mark:                     |
| Arduino Leonardo | :x:           | :heavy_check_mark:         | :heavy_check_mark:                     |

## Interconnection
LoRa RFM95 works through SPI Connections. The SPI connections compose of MOSI/COPI, MISO/CIPO, and SCK. Each thus three pins varies for every development boards. The below examples used the below connections, if your development board is not listed, does not mean it cannot connect to the LoRa Breakout. It only means we have not tried it for any reasons. It might still work. 

| Development Board    | LoRa Breakout                | MOSI | MISO | SCK  | RST  | NSS  | DIO0 | DIO1 |
|----------------------|------------------------------|------|------|------|------|------|------|------|
| ESP32                | Variant 3.3V & Variant Dual  | IO13 | IO12 | IO14 | IO26 | IO15 | IO27 | NC   | 
| Arduino Uno R3       | Variant 5V & Variant Dual    | 11   | 12   | 13   | 9    | 10   | 2    | 6    |
| Arduino Mega R3      | Variant 5V & Variant Dual    | 51   | 50   | 53   | 9    | 10   | 2    | 6    |
| Arduino Leonardo     | Variant 5V & Variant Dual    | 11   | 12   | 13   | 9    | 10   | 2    | 6    |

## Examples
On Going

Useful resources of https://www.tokopedia.com/cosmic-iot/lora-chip-breakout-pcb-untuk-rfm95-rfm96-rfm-95-96-dengan-chip-ufl-5v-tanpa-antena
