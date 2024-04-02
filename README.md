# Ambient_temp_control_using_fuzzyset
Code explaination 
1. Membership Functions:
 fuzzy_membership_temperature(temperature): This function takes the ambient temperature as input and returns the membership values for three fuzzy sets: cold, warm, and hot. These membership values represent the degree to which the temperature belongs to each fuzzy set.
 fuzzy_membership_power(power): Similar to the previous function, this function takes the power level as input and returns the membership values for three fuzzy sets: low, medium, and high.

  2. Rules:
fuzzy_rule_base(temperature): This function represents the rule base of the fuzzy system. It takes the membership values of the temperature fuzzy sets as input and determines the appropriate power level based on these values. For example, if the temperature is cold, the power level should be high; if it's warm, the power level should be medium; and if it's hot, the power level should be low.

3. Defuzzification:
defuzzify(power): This function takes the fuzzy power levels (as determined by the rule base) and calculates the crisp output power level. It uses the centroid method for defuzzification, where the weighted average of the power levels is computed based on the membership values of each power level.

4.Controller:
fuzzy_controller(temperature): This function represents the overall fuzzy controller. It takes the ambient temperature as input, determines the membership values for the temperature fuzzy sets, applies the rules to determine the power level, and then defuzzifies the result to obtain the crisp output power level.
