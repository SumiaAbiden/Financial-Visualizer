def CheckIfFloat(x):
    if x.replace(".", "").isnumeric():
        return True
    

def percentage(x, salary):
    percentage = x/salary * 100
    return percentage


print('--------------------------------')
print('----- FINANCIAL VISUALIZER -----')
print('--------------------------------')

salary = input('Annual Salary:\n')
housing = input('Monthly Housing:\n')
bills = input('Monthly Bills:\n')
food = input('Weekly Food:\n')
travel = input('Annual Travel:\n')


if CheckIfFloat(salary) and CheckIfFloat(housing) and CheckIfFloat(bills) and CheckIfFloat(food) and CheckIfFloat(travel):
    print("All inputs confirmed valid.")
    salary = float(salary)
    
    if salary<=10000:
        tax = round(salary*0.05 , 2)
    elif salary<=40000:
        tax = round(salary*0.1 , 2)
    elif salary<=80000:
        tax = round(salary*0.15 , 2)
    elif salary>80000:
        tax = round(salary*0.2 , 2)

    
    
    housing = float(housing)*12
    bills = float(bills)*12
    food = float(food)*52
    travel = float(travel)
    tax = float(tax)

    extra = salary - (housing + bills + food + travel + tax)
    

    print("\n\n-----------------------------------------------------------------------------------")
    print("housing | $" , format(housing, '11,.2f') , " | " , format(percentage(housing, salary), '5,.1f')  , '% | ' , ('#' * int(percentage(housing, salary))))
    print("  bills | $" , format(bills, '11,.2f') , " | " , format(percentage(bills, salary), '5,.1f')  , '% | ' , ('#' * int(percentage(bills, salary))))
    print("   food | $" , format(food, '11,.2f') , " | " , format(percentage(food, salary), '5,.1f')  , '% | ' , ('#' * int(percentage(food, salary))))
    print(" travel | $" , format(travel, '11,.2f') , " | " , format(percentage(travel, salary), '5,.1f')  , '% | ' , ('#' * int(percentage(travel, salary))))
    print("    tax | $" , format(tax, '11,.2f') , " | " , format(percentage(tax, salary), '5,.1f')  , '% | ' , ('#' * int(percentage(tax, salary))))
    print("  extra | $" , format(extra, '11,.2f') , " | " , format(percentage(extra, salary), '5,.1f')  , '% | ' , ('#' * int(percentage(extra, salary))))
    print("-----------------------------------------------------------------------------------")

else:
    print("Invalid input, please try again.")



