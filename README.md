

days = int(input("Enter the number of days: "))
years = days // 365
weeks = (days % 365) // 7
remaining_days = (days % 365) % 7
print("days:-",days)
print("years:-",years)
print("weeks:-",weeks)
print("remaining days:-",remaining_days)
# que:-2

basic_salary = float(input("Enter the basic salary of the employee: "))
if basic_salary <= 10000:
    HRA = 0.20 * basic_salary
    DA = 0.80 * basic_salary
elif basic_salary <= 20000:
    HRA = 0.30 * basic_salary
    DA = 0.90 * basic_salary
else:
    HRA = 0.35 * basic_salary
    DA = 0.95 * basic_salary
gross_salary = basic_salary + HRA + DA
print(f"Basic Salary: {basic_salary}")
print("HRA:-",HRA)
print("DA:-",DA)
print("Gross Salary:-",gross_salary)
# que:-3 (doubt) 

units = float(input("Enter the number of electricity units consumed: "))
total_bill = 0
if units <= 50:
    total_bill = units * 0.50
elif units <= 150:
    total_bill = (50 * 0.50) + ((units - 50) * 0.75)
elif units <= 250:
    total_bill = (50 * 0.50) + (100 * 0.75) + ((units - 150) * 1.25)
else:
    total_bill = (50 * 0.50) + (100 * 0.75) + (100 * 1.25) + ((units - 250) * 1.50)
perc = (17 / total_bill) * 100
surcharge = total_bill + perc
total_bill += surcharge

print("Electricity units consumed:-",units)
print("Total bill amount (including surcharge): Rs:",total_bill)
# que :- 4


num_rows =5
for i in range(1, num_rows + 1):
 for j in range(i):
        print(i, end=" ")
    
 print()
 # que 5

n = int(input("Enter a number: "))
product = 1
while n > 0:
    digit = n % 10  
    product *= digit
    n //= 10


print("The product of the digits is:=",product)
# que 6


x = [45,67,12,'hello',23.45,'world']
