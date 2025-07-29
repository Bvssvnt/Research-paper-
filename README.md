# BMI Calculator
def calculate_bmi(weight, height):
    bmi = weight / (height ** 2)
    if bmi < 18.5:
        return "Underweight"
    elif bmi < 25:
        return "Normal weight"
    elif bmi < 30:
        return "Overweight"
    else:
        return "Obese"

weight = float(input("Enter your weight (kg): "))
height = float(input("Enter your height (m): "))
result = calculate_bmi(weight, height)
print("Your BMI category is:", result)
