# BMI-Calculator



def calculate_bmi(weight,height):
    bmi= weight / (height ** 2) 
    return bmi

def bmi_category(bmi):

    if bmi < 18.5 :
        return "Underweight"
    elif 18.5 <= bmi < 24.9:
        return "Healthy Weight"
    elif 25 <= bmi < 29.9:
        return "Overweight"
    else:
        return "Obesity"

weight = float(input("Enter your weight in kilograms : "))
height = float(input("Enter your height in meters : "))

bmi = calculate_bmi(weight,height)

print("Your BMI is : ",bmi)
print("Category : ",bmi_category(bmi))
