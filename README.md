# Grade-calculator.
Python project to calculate based on marks 
# grade_calculator.py

# Get student details
name = input("Enter your name: ")
roll = input("Enter your roll number: ")

# Input 5 subject marks
print("\nEnter marks out of 100:")
marks = []
for i in range(1, 6):
    mark = int(input(f"Subject {i}: "))
    marks.append(mark)

# Calculations
total = sum(marks)
average = total / 5

# Grade logic
if average >= 90:
    grade = 'A+'
elif average >= 80:
    grade = 'A'
elif average >= 70:
    grade = 'B'
elif average >= 60:
    grade = 'C'
elif average >= 50:
    grade = 'D'
else:
    grade = 'F (Fail)'

# Result
print("\n----- Report Card -----")
print(f"Name        : {name}")
print(f"Roll No     : {roll}")
print(f"Total Marks : {total} / 500")
print(f"Average     : {average:.2f}")
print(f"Grade       : {grade}")
