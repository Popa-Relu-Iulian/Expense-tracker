#Expense tracker

expenses = [] # we create the empty list

for i in range(5):
    daily_expenses = float(input("Enter 5 daily expenses, in numbers:"))
    expenses.append(daily_expenses)
    
print("\nYour expenses are:")

# We created the question loop

for i, expense in enumerate(expenses, start= 1):
    print(f"{i}. {expense}")
    
# We create the remove index

remove_index = int(input("Which number on the list you would like to remove?"))
removed_expense = expenses.pop(remove_index -1)
print(f"Removed: {removed_expense}")

print(f"Now your list is: {expenses}")

total = sum(expenses)
highest = max(expenses)
lowest = min(expenses)
average = sum(expenses) / len(expenses)

print(f"The total is: {total}")
print(f"The highest is: {highest}")
print(f"The lowest is: {lowest}")
print(f"The average is: {average}")
