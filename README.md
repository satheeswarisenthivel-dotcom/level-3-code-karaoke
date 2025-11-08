
<img width="5400" height="2383" alt="Code Karaoke-min" src="https://github.com/user-attachments/assets/cf9296ba-8410-4592-8df0-bac4afd7fdba" />

# Level-3-code-karaoke
Level 3 questions for code karaoke event, there are 2 scenario based  fork and upload in git hub 

# 1st Question :
1.You are building a billing system for a small café.
The café sells:
•	Coffee → ₹60
•	Sandwich → ₹120
•	Cake → ₹80
You need to write a Python program that:
1.	Asks the user what they want to order.
2.	Asks how many of that item they want.
3.	Calculates and displays the total bill.

# Code:menu = {
    "coffee": 60,
    "sandwich": 120,
    "cake": 80
}

print("Welcome to the Café!")
print("Menu:")
for item, price in menu.items():
    print(f"{item.capitalize()} - ₹{price}")


order = input("\nWhat would you like to order? ").lower()


if order in menu:
    quantity = int(input(f"How many {order}s would you like? "))
    total = menu[order] * quantity
    print(f"\nYour total bill for {quantity} {order}(s) is ₹{total}.")
else:
    print("\nSorry, that item is not on the menu.")

# OUTPUT:
<img width="1920" height="1080" alt="Screenshot (157)" src="https://github.com/user-attachments/assets/cdcdfce7-8a07-4990-9b37-5613b5626189" />
<img width="1920" height="1080" alt="Screenshot (156)" src="https://github.com/user-attachments/assets/8092b252-5f90-42a8-aa47-f1e69b99faa4" />


# Question 2:
2. You’re designing a program for a college portal that evaluates a student’s final grade based on their marks in 3 subjects.
Rules:
•	If the average is 90 or above → Grade A+
•	If the average is 75–89 → Grade A
•	If the average is 60–74 → Grade B
•	If the average is 40–59 → Grade C
•	Below 40 → Fail
The program should:
1.	Take marks for 3 subjects from the user
2.	Calculate the average
3.	Print the average and the grade
________________________________________
# Example Input / Output:
Enter mark for Subject 1: 85
Enter mark for Subject 2: 78
Enter mark for Subject 3: 90
Average = 84.33
Grade = A





# Code:
mark1 = float(input("Enter mark for Subject 1: "))
mark2 = float(input("Enter mark for Subject 2: "))
mark3 = float(input("Enter mark for Subject 3: "))

average = (mark1 + mark2 + mark3) / 3

if average >= 90:
    grade = "A+"
elif average >= 75:
    grade = "A"
elif average >= 60:
    grade = "B"
elif average >= 40:
    grade = "C"
else:
    grade = "Fail"

print(f"Average = {average:.2f}")
print(f"Grade = {grade}")


# OUTPUT:
<img width="1920" height="1080" alt="Screenshot (160)" src="https://github.com/user-attachments/assets/f31ee3d6-26cf-4a53-a388-d6e2b5f98d9e" />

<img width="1920" height="1080" alt="Screenshot (161)" src="https://github.com/user-attachments/assets/670ae6fb-e33b-4ceb-bd3e-e118df845068" />


