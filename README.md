def main():
    while True:
        print("\nStudent Result Management System")
        print("1.Add Student")
        print("2.Add Course")
        print("3.Add Result")
        print("4.Generate Student Report")
        print("5.Generate Course Report")
        print("6.Exit")
    choice = int(input("enter your choice"))
    if choice ==1:
        name = input("Enter Student name")
        age = int(input("Enter Student age"))
        gender = input("Enter Student gender:")
        add_student(name,age,gender)
    elif choice ==2:
        course_name = input("Enter course name:")
        instructor = input("Enter instructor name:")
        add_course(course_name,instructor)
    elif choice ==3:
        student_id=int(input("Enter student ID:"))
        course_id=int(input("Enter course ID:"))
        marks=int(input("Enter marks:"))
        add_result(student_id,course_id,marks)
    elif choice ==4:
        student_id=int(input("Enter student ID to generate report:"))
        generate_student_report(student_id) 
    elif choice ==5:
        course_id=int(input("Enter course ID to generate report"))
        generate_course_report(course_id)
    elif choice ==6:
        print("Exiting the system...")
    else:
        print("invalid choice! please try again.")
        main()
     #def view_statement():
        for s in students:
            print(s)# Student-management-
Record 
