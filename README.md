  print("Welcome to MR_FANCI art gallery")
while True:
    print("\nWhich shape do you want to draw?")
    print("1. Triangle")
    print("2. Diamond")
    print("3. Exit")
    choice = input("Enter your choice (1, 2, or 3): ")
    if choice == "3":
        print("Thank you for visiting MR_FANCI art gallery!")
        break
    custom_word = input("Enter the word you want to write instead of * in your selected shape: ")
    if choice == "1":
        print("Which triangle do you want?")
        print("1. Upright")
        print("2. Inverted")
        choice2 = input("Enter your choice (1 or 2): ")
        rows = int(input("Enter the number of rows: "))
        if choice2 == "1":
            for i in range(1, rows + 1):
                print(" " * (rows - i) + (custom_word + " ") * i)
        elif choice2 == "2":
            for i in range(rows, 0, -1):
                print(" " * (rows - i) + (custom_word + " ") * i)
        else:
            print("Invalid triangle choice.")
    elif choice == "2":
        rows = int(input("Enter the no. of rows: "))
    for i in range(1, rows + 1):
        print(" " * (rows - i) + (custom_word + " ") * i)
    for j in range(rows - 1, 0, -1):
        print(" " * (rows - j) + (custom_word + " ") * j)
else:
    print("Invalid choice.")
    print("Invalid choice.")
