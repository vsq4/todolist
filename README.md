tasks = []
ask = input("Enter an activity ")
tasks.append(ask)
next = input("Would you like to add more activities? ").strip().lower() 
while next == "yes":
    other = input("Enter a new activity ").strip().lower() 
    if other == "end":
        break
    tasks.append(other)
print(f"Your to do list consists of: {', '.join(tasks)}")
