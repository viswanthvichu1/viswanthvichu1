
def celsius_to_fahrenheit(celsius):
return (celsius * 9/5) + 32
def fahrenheit_to_celsius(fahrenheit):
return (fahrenheit - 32) * 5/9
def celsius_to_kelvin(celsius):
return celsius + 273.15
def kelvin_to_celsius(kelvin):
return kelvin - 273.15
def fahrenheit_to_kelvin(fahrenheit):
return (fahrenheit - 32) * 5/9 + 273.15
def kelvin_to_fahrenheit(kelvin):
return (kelvin - 273.15) * 9/5 + 32

def meters_to_kilometers(meters):
return meters / 1000
def kilometers_to_miles(kilometers):
return kilometers * 0.621371
def miles_to_kilometers(miles):
return miles / 0.621371
def kilograms_to_pounds(kilograms):
return kilograms * 2.20462
def pounds_to_kilograms(pounds):
return pounds / 2.20462

def main():
print("Welcome to the Converter Program!")
print("Select the type of conversion:")
print("1. Temperature Converter")
print("2. Measurement Converter")
choice = int(input("Enter your choice (1 or 2): "))
if choice == 1:
print("\nTemperature Converter")
print("1. Celsius to Fahrenheit")
print("2. Fahrenheit to Celsius")
print("3. Celsius to Kelvin")
print("4. Kelvin to Celsius")
print("5. Fahrenheit to Kelvin")
print("6. Kelvin to Fahrenheit")
temp_choice = int(input("Select the conversion (1-6): "))
temp = float(input("Enter the temperature to convert: "))
if temp_choice == 1:
print(f"{temp} Celsius = {celsius_to_fahrenheit(temp)} Fahrenheit")
elif temp_choice == 2:
print(f"{temp} Fahrenheit = {fahrenheit_to_celsius(temp)} Celsius")
elif temp_choice == 3:
print(f"{temp} Celsius = {celsius_to_kelvin(temp)} Kelvin")
elif temp_choice == 4:
print(f"{temp} Kelvin = {kelvin_to_celsius(temp)} Celsius")
elif temp_choice == 5:
print(f"{temp} Fahrenheit = {fahrenheit_to_kelvin(temp)} Kelvin")
elif temp_choice == 6:
print(f"{temp} Kelvin = {kelvin_to_fahrenheit(temp)} Fahrenheit")
else:
print("Invalid choice!")
elif choice == 2:
print("\nMeasurement Converter")
print("1. Meters to Kilometers")
print("2. Kilometers to Miles")
print("3. Miles to Kilometers")
print("4. Kilograms to Pounds")
print("5. Pounds to Kilograms")
measure_choice = int(input("Select the conversion (1-5): "))
value = float(input("Enter the value to convert: "))
if measure_choice == 1:
print(f"{value} meters = {meters_to_kilometers(value)} kilometers")
elif measure_choice == 2:
print(f"{value} kilometers = {kilometers_to_miles(value)} miles")
elif measure_choice == 3:
print(f"{value} miles = {miles_to_kilometers(value)} kilometers")
elif measure_choice == 4:
print(f"{value} kilograms = {kilograms_to_pounds(value)} pounds")
elif measure_choice == 5:
print(f"{value} pounds = {pounds_to_kilograms(value)} kilograms")
else:
print("Invalid choice!")
else:
print("Invalid choice! Please select either 1 or 2.")
# Run the program
if __name__ == "__main__":
main()
OUTPUT:
Welcome to the Converter Program!
Select the type of conversion:
1. Temperature Converter
2. Measurement Converter
Enter your choice (1 or 2): 2
Measurement Converter
1. Meters to Kilometers
2. Kilometers to Miles
3. Miles to Kilometers
4. Kilograms to Pounds
5. Pounds to Kilograms
Select the conversion (1-5): 4
Enter the value to convert: 5
5.0 kilograms = 11.0231 pounds
