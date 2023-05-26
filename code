# This code allows a specified number of students to register for an exam
# The user inputs their student number
# The student numbers are added to a text file along with a dotted line, allowing them to sign next to their student number.


# A while True is used, along with a try and except to ensure the user only inputs an integer.

while True:
    try:
        number_students = int(input("How many students are registering for the exam? "))
        break

    except ValueError as error:
       print("ERROR: Please enter an integer")
       print(error)

# The code writes to a text file called reg_form
with open("reg_form.txt", 'w') as file:


# This part of the code ensures that the students are inputting valid student numbers. 
# If they input a letter they will recieve an error message.
    for student in range(number_students):
        while True:
            try:
                student_id = int(input("Please enter your student ID number: "))
                break
            
            except ValueError as error:
                print("ERROR: Please enter a valid ID number")
                print(error)
        file.write(str(student_id))
        file.write(" ..............................................\n")
