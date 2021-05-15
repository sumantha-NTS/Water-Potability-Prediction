# Water-Potability-Prediction
Prediction of water potability with parameters like ph, hardness, turbidity etc.

## Background:
“Potable water” simply means water that is safe to drink, and it is becoming scarcer in the world. Increasing use is stressing freshwater resources worldwide, and a seemingly endless list of contaminants can turn once potable water into a health hazard or simply make it unacceptable aesthetically.

### What Makes Water Unsuitable for Drinking?
The World Health Organization (WHO) organizes potable water contamination as organic, inorganic, radiological, and microbiological, and includes measures of acceptability of taste, smell, and appearance.
1. Organic contaminants are carbon-based chemicals, including solvents and pesticides, which are introduced through agricultural runoff or industrial discharge. They can be responsible for a range of severe health problems from cancer to endocrine function disruption.
2. Radiological threats include radon, cesium, plutonium and uranium. In North America, radon is the leading cause of lung cancer in nonsmokers and the leading environmental cause of cancer mortality overall.
3. Inorganic pollutants, such as mineral acids, inorganic salts, metals, cyanides, and sulfates, persist in the environment. Heavy metals can cause neurological problems in humans, especially in the unborn and children, and also bio-accumulate in some foods. Arsenic can cause cancer, skin lesions, cardiovascular disease, diabetes, and cognitive impairment. Algal blooms from nutrients like phosphorus and nitrogen can also introduce cyanotoxins to drinking water as well.

## Dataset:
The dataset considered for this project is taken from Kaggle dataset. Link is given below\
https://www.kaggle.com/adityakadiwal/water-potability

## Dataset details:
Dataset consists of 3276 records with 10 column of which 9 are input variables and 'potability' is the output variable.

### Variable details:
All the variables in the dataset are explained below.
1. **pH Value:** PH is an important parameter in evaluating the acid–base balance of water. It is also the indicator of acidic or alkaline condition of water status. WHO has recommended maximum permissible limit of pH from 6.5 to 8.5. The current investigation ranges were 6.52–6.83 which are in the range of WHO standards.
2. **Hardness:** Hardness is mainly caused by calcium and magnesium salts. These salts are dissolved from geologic deposits through which water travels. The length of time water is in contact with hardness producing material helps determine how much hardness there is in raw water. Hardness was originally defined as the capacity of water to precipitate soap caused by Calcium and Magnesium.
3. **Solids (Total dissolved solids - TDS):** Water has the ability to dissolve a wide range of inorganic and some organic minerals or salts such as potassium, calcium, sodium, bicarbonates, chlorides, magnesium, sulfates etc. These minerals produced un-wanted taste and diluted color in appearance of water. This is the important parameter for the use of water. The water with high TDS value indicates that water is highly mineralized. Desirable limit for TDS is 500 mg/l and maximum limit is 1000 mg/l which prescribed for drinking purpose.
4. **Chloramines:** Chlorine and chloramine are the major disinfectants used in public water systems. Chloramines are most commonly formed when ammonia is added to chlorine to treat drinking water. Chlorine levels up to 4 milligrams per liter (mg/L or 4 parts per million (ppm)) are considered safe in drinking water.
5. **Sulfate:** Sulfates are naturally occurring substances that are found in minerals, soil, and rocks. They are present in ambient air, groundwater, plants, and food. The principal commercial use of sulfate is in the chemical industry. Sulfate concentration in seawater is about 2,700 milligrams per liter (mg/L). It ranges from 3 to 30 mg/L in most freshwater supplies, although much higher concentrations (1000 mg/L) are found in some geographic locations.
6. **Conductivity:** Pure water is not a good conductor of electric current rather’s a good insulator. Increase in ions concentration enhances the electrical conductivity of water. Generally, the amount of dissolved solids in water determines the electrical conductivity. Electrical conductivity (EC) actually measures the ionic process of a solution that enables it to transmit current. According to WHO standards, EC value should not exceeded 400 μS/cm.
7. **Organic_carbon:** Total Organic Carbon (TOC) in source waters comes from decaying natural organic matter (NOM) as well as synthetic sources. TOC is a measure of the total amount of carbon in organic compounds in pure water. According to US EPA < 2 mg/L as TOC in treated / drinking water, and < 4 mg/Lit in source water which is use for treatment.
8. **Trihalomethanes:** THMs are chemicals which may be found in water treated with chlorine. The concentration of THMs in drinking water varies according to the level of organic material in the water, the amount of chlorine required to treat the water, and the temperature of the water that is being treated. THM levels up to 80 ppm is considered safe in drinking water.
9. **Turbidity:** The turbidity of water depends on the quantity of solid matter present in the suspended state. It is a measure of light emitting properties of water and the test is used to indicate the quality of waste discharge with respect to colloidal matter. The mean turbidity value obtained for Wondo Genet Campus (0.98 NTU) is lower than the WHO recommended value of 5.00 NTU.

Finally, **Potability** is the output variable which represents the water is drinkable or not.

## Exploratory data analysis(EDA):
There are missing values in the dataset. All the missing values are imputed with different techniques.
After imputation of missing values, EDA is performed on the dataset and got few insights. For detailed explaination please refer python file present in this repository.

## Model Building and Evaluation:
Different models are built and are optimized with hyper parameters using GridSearchCV. The results are shown below
