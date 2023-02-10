# BITS-Steel-Industry-Energy-Consumption
# analysis-Steel-Industry-Energy-Consumption
The attempt here is to analyze the factors responsible for energy load, What Factor which triggered an energy load that is classified as a maximum load, how effectively the energy load has been consumed.

# Dataset Information
This dataset is data on the energy load consumed by DAEWOO Steel Co. Ltd  for 1 year (2018)

# Objective
Energy consumption is one of the important aspects in the industrial world. The more effectively the energy is consumed, the more efficient the costs incurred. This project presents an analysis of what factors most influence the Type of Energy Load and What Factor which triggers an energy load that is classified as a maximum load also how effectively the energy load has been consumed

# Attribute Information
1. Date – datetime per 15 minutes
2. Usage_kWh = Industry Energy Consumption - Continuous (kWh)
3. Lagging_Current_Reactive.Power_kVarh = Lagging Current reactive power - Continuous (kVarh)
4. Leading_Current_Reactive_Power_kVarh = Leading Current reactive power - Continuous (kVarh)
5. CO2(tCO2) = rate of CO2(CO2) - Continuous (ppm)
6. Lagging_Current_Power_Factor = Lagging Current power factor -Continuous (%)
7. Leading_Current_Power_Factor = Leading Current Power factor Continuous - (%)
8. NSM  = Number of Seconds from midnight Continuous - (s)
9. WeekStatus= Week status - Categorical (Weekend (0) or a Weekday(1))
10. Day_of_week= Day of week - Categorical Monday to Sunday
11. Load_Type= Load Type - Categorical Light Load, Medium Load, Maximum Load

# Step
1. Make sure the csv file and the code in one folder

# Insight
1. Sunday is the day with the lightest energy use
2. Light_load energy usage increases as the day progresses (closer to Sunday)


3. From the three graphs above, usage_kWh, Lagging_Current_Reactive.Power_kVarh and CO2, have a tendency to increase at maximum load. It can be seen that these 3 factors have a fairly high graph at maximum load

4. From modeling, it can be seen that the NSM has the largest value, it means NSM has high contribution to prediction/target column


# Conclusion
1. NSM is the most influencing factor for the type of energy load
2. The closer to the weekend, the lighter the energy load
3. Usage_kWh, Lagging_Current_Reactive.Power_kVarh and CO2 triggered an energy load that is classified as a maximum load
4. SHAP Feature Importance where this method will provide SHAP (SHapley Additive ExPlanations) values which are based on cooperative game theory and are used to increase transparency and interpretation of machine learning models. From the 3 summary plots above, all of them show the same thing, so the conclusions from the modeling are considered the same as the conclusions from the EDA that has been done
5. When viewed from the energy load distribution plot, it can be seen that the light load has the highest number among the others. So, it can be said that energy consumption for 2018 is still considered effective

