# Microclimatic Data for two Tunnel Greenhouses in northern-east Italy

## Authors
Elia Brentarolli<sup>1*</sup>, Silvia Locatelli<sup>2</sup>, Carlo Nicoletto<sup>2</sup>, Paolo Sambo<sup>2</sup>, Davide Quaglia<sup>1</sup>, Riccardo Muradore<sup>3</sup>

<sup>1</sup> Department of Computer Science, University of Verona, Verona, Italy

<sup>2</sup> DAFNAE department - University of Padua, Padua, Italy

<sup>3</sup> Department of Engineering for Innovation Medicine (DIMI), University of Verona,
Verona, Italy

<sup>*</sup> elia.brentarolli@univr.it
## Summary
The  dataset contains data collected from various sensors positioned in two different greenhouses in different farms in northern-east Italy. Data collected focus on the microclimate of each greenhouse. Most data focuses on monitoring air temperature in different position of the same greenhouse, hence most data refers to such measure. However, other measures were also taken, and reported in the files. Additionally, data outside the two greenhouses were also taken via two distinct weather stations.

## Keywords
Microclimate, Weather Data, Climate Modeling

## Abstract
Greenhouse internal microclimate has been proven to be non-homogeneous in many aspects. However, this variability is only sometimes considered by greenhouse models, which often calculate climatic variables without any spatial reference. Farmers, on the other hand, may wish to have these differences highlighted as they could lead to aimed actions only for a specific area of the greenhouse, while at the same time, they are not willing to invest in sensors to be installed everywhere. 

This paper presents a data-driven methodology to generate a virtual 2D map of a greenhouse, which allows farmers to control any critical parameter they desire with minimum investment, as monitoring is done via soft sensing with only a few actual sensors. The proposed flow starts with a set of temporary sensors placed in the points of interest; then, a model for each of them is developed via linear regression and, finally, a map of the entire area can be derived by interpolating values from these models. This allows the generation of accurate models at a reduced cost as temporary sensors can be reused at other locations. The methodology has been tested on adjacent greenhouses and in two farms, where temperature and other climatic variables have been monitored. Experimental results show that the proposed methodology can reach an adjusted R<sup>2</sup> value of 98% for predicting values in different greenhouse locations.

## Description of the data and file structure

For each greenhouse, a folder is provided containing all data retrieved from sensors inside it, as well as from the station outside. Naming for files is given according to the following convention:
*   The `Micro_*` series contains microclimatic data retrieved from a data logger positioned near the crops. It contains measure **Plant and Soil Temperature**, **PAR**, and two simultaneous readings for **Soil Water Content**
*   The `Ref_*` series stores data from a fixed climatic station we used as reference throughout our experiment, hence the naming. Each `Ref` file is followed by the measure it stores (e.g. `Ref_AirTemp` has data related to air temperature, `Ref_RH` to air humidity etc.)
*   The `Temp_4ch_*` series stores data from a 4-channel data logger equipped with four distinct **air temperature** sensors.
*   The `TRH_*` files stores data for **air temperature** and **humidity**
*   The `weather_station` files contains all readings from the external weather station
*   Only for *greenhouse_1*: the `Valid_*` files store more air temperature data retrieved from other points of the greenhouse used for validation

## Founding
The data were collected within the project "L’agricoltura del futuro e gli alimenti funzionali: una sfida per la ricerca e il rilancio del territorio veneto" funded by Regione del Veneto under POR FESR 2014-2020 Action 1.1.4 (ID 10288429).
