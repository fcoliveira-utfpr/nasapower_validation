# Validation of NASA/POWER data for estimating ETo
This project presents the codes and dataset used for data analysis in the development of the article titled **"How accurate are the NASA/POWER data for estimating reference evapotranspiration in humid climate regions in Brazil?"**. The analyses were conducted in Google Colab.

# How to cite?
GIOVANELLA, T. H.; OLIVEIRA, F. C.; SOBUCKI, L.; SERVÍN NIZ, A. I. How accurate are the NASA/POWER data for estimating reference evapotranspiration in humid climate regions in Brazil? Título do Periódico, [local], v. x, n. x, p. xx-xx, ano. DOI: [inserir].

# ABSTRACT
Global atmospheric models that provide gridded data present themselves as a reliable option for filling gaps in meteorological station data and for climate monitoring in various areas of the world. Additionally, they provide the necessary data for reference evapotranspiration estimates. However, it is essential to assess the performance of these models for local and regional applications. In this regard, this research aimed to evaluate the accuracy of NASA/POWER reanalysis data and its performance for reference evapotranspiration estimates in humid climate regions in Brazil. Ten years of meteorological data from surface stations were compared with NASA/POWER data. Aditionally, three methods for estimating reference evapotranspiration were analyzed, consistently comparing station data with reanalysis data. The comparison between the data series was conducted considering the following statistical indices: Pearson correlation coefficient, Wilmott's concordance, Mean Absolute Error, and Root Mean Square Error. It was observed that NASA/POWER meteorological variables such as maximum temperature, minimum temperature, global solar radiation, and top-of-atmosphere radiation provided more accurate estimates than relative humidity and wind speed, which exhibited larger estimation errors. The Penman-Monteith method demonstrated the lowest estimation errors for determining reference evapotranspiration using NASA/POWER data. Determining reference evapotranspiration using NASA/POWER data with a constant wind speed of 2.0 m/s resulted in higher accuracy in evapotranspiration estimates. 

# Repository Contents
`dados_ET.csv`: contains daily evapotranspiration data, calculated for the following municipalities: 'Sete Quedas', 'Planalto', 'Nova Tebas', 'Maringá', 'Marechal Cândido Rondon', 'Foz do Iguaçu', and 'Cidade Gaúcha'. It was determined for surface station data (ETo sur), NASA/POWER data (ETo NP), and NASA/POWER data with constant wind speed at 2 m/s (ETo U2.0).
`dados_ET.csv`: 
| Variable (CSV Header) | Description | Unit |
| :--- | :--- | :--- |
| **YEAR** | Year | - |
| **DOY** | Day of the Year | 1 to 365/366 |
| **ALLSKY_SFC_SW_DWN** | All-sky Surface Shortwave Downward Irradiance | MJ/m²/day |
| **T2M_MIN** | Minimum Air Temperature at 2m | °C |
| **T2M_MAX** | Maximum Air Temperature at 2m | °C |
| **PRECTOTCORR** | Corrected Total Precipitation | mm/day |
| **RH2M** | Relative Humidity at 2m | % |
| **U2** | Wind Speed at 2m (Original NASA/POWER) | m/s |
| **Tmed** | Mean Air Temperature | °C |
| **UR Med (%)** | Mean Relative Humidity | % |
| **es** | Saturation Vapor Pressure | kPa |
| **s** | Slope of Saturation Vapor Pressure Curve | kPa/°C |
| **ea** | Actual Vapor Pressure | kPa |
| **Declinação solar** | Solar Declination | rad |
| **N -fotoperíodo (horas)** | Photoperiod (Daylight Hours) | hours |
| **NDA** | Number of Days in the Year | - |
| **H ângulo horário (graus)** | Sunset Hour Angle | degrees |
| **(d/D)²** | Inverse Relative Earth-Sun Distance Squared | - |
| **Irradiância solar extraterrestre (Qo=RA)  (MJ/m²d)** | Extraterrestrial Solar Radiation | MJ/m²/day |
| **BOC** | Net Shortwave Radiation | MJ/m²/day |
| **Qg CS** | Net Longwave Radiation | MJ/m²/day |
| **BOL** | Net Radiation (Longwave Balance) | MJ/m²/day |
| **Rn** | Net Radiation (Penman-Monteith Method) | MJ/m²/day |
| **Eto - PM (mm/d)** | Reference Evapotranspiration (Intermediate Calculation) | mm/day |
| **latitude** | Station Latitude | decimal degrees |
| **altitude** | Station Altitude | m |
| **Municipio** | Municipality Name | - |
| **ETo_superficie** | Reference Evapotranspiration from Surface Station | mm/day |
| **Patm** | Atmospheric Pressure | kPa |
| **gama** | Psychrometric Constant | kPa/°C |
| **U_0_5** | Constant Wind Speed at 0.5 m/s | m/s |
| **U_1** | Constant Wind Speed at 1.0 m/s | m/s |
| **U_1_5** | Constant Wind Speed at 1.5 m/s | m/s |
| **U_2** | Constant Wind Speed at 2.0 m/s | m/s |
| **ETo_PM_NP** | ETo (Penman-Monteith with NASA/POWER Data) | mm/day |
| **ETo_U05** | ETo (Constant Wind Speed U2 = 0.5 m/s) | mm/day |
| **ETo_U1** | ETo (Constant Wind Speed U2 = 1.0 m/s) | mm/day |
| **ETo_U1_5** | ETo (Constant Wind Speed U2 = 1.5 m/s) | mm/day |
| **ETo_U2** | ETo (Constant Wind Speed U2 = 2.0 m/s) | mm/day |
| **ETo_PM_sup** | ETo (Penman-Monteith with Surface Station Data) | mm/day |

