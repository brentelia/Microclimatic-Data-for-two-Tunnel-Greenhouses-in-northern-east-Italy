# Microclimatic Data for two Tunnel Greenhouses in northern-east Italy

The dataset contains data collected from various sensors positioned in two different greenhouses in different farms in northern-east Italy. Data collected focus on the microclimate of each greenhouse. Most data focuses on monitoring air temperature in different position of the same greenhouse, hence most data refers to such measure. However, other measures were also taken, and reported in the files. Additionally, data outside the two greenhouses were also taken via two distinct weather stations.

## Description of the data and file structure

For each greenhouse, a folder is provided containing all data retrieved from sensors inside it, as well as from the station outside. Naming for files is given according to the following convention:
*   The `Micro_*` series contains microclimatic data retrieved from a data logger positioned near the crops. It contains measure **Plant and Soil Temperature**, **PAR**, and two simultaneous readings for **Soil Water Content**
*   The `Ref_*` series stores data from a fixed climatic station we used as reference throughout our experiment, hence the naming. Each `Ref` file is followed by the measure it stores (e.g. `Ref_AirTemp` has data related to air temperature, `Ref_RH` to air humidity etc.)
*   The `Temp_4ch_*` series stores data from a 4-channel data logger equipped with four distinct **air temperature** sensors.
*   The `TRH_*` files stores data for **air temperature** and **humidity**
*   The `weather_station` files contains all readings from the external weather station
*   Only for *greenhouse_1*: the `Valid_*` files store more air temperature data retrieved from other points of the greenhouse used for validation
