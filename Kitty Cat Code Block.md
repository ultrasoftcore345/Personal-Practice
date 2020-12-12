# Bonus

Throw this baby in a shell and have yourself a short kitty adventure:

```
do_calculation = True

while (do_calculation):

    print("\nThe Escape \n \n")

    print("Oh no! Old Man Jenkins' kitty cat, Mr. Socks, is running away from home!")
    print("Luckily, you happen to have super vision and are able to determine the cat's starting distance and speed, rate of acceleration, and how long he ran. This will help you determine how far from home he is.")
    print("As we know, with great power comes great responsibility. Help your neighbor figure out how far Mr. Socks ran! \n \n")

    while(True):
        try:
            initial_position = float(input("\nEnter how far Mr. Socks started from home as a whole number or decimal value (meters): "))
        except ValueError:
            print("Only numerical values are valid. Please enter a valid value.")
            continue
        else:
            break

    while(True):
        try:
            initial_velocity = float(input("\nEnter how fast Mr. Socks started running as a whole number or decimal value (meters/second): "))
        except ValueError:
            print("Only numerical values are valid. Please enter a valid value.")
            continue
        else:
            break

    while(True):
        try:
            acceleration_rate = float(input("\nEnter how fast Mr. Socks accelerated as a whole number or decimal value (meters/second): "))
        except ValueError:
            print("Only numerical values are valid. Please enter a valid value.")
            continue

        else:
            break
        
    while(True):
        try:
            travel_time = float(input("\nEnter how long Mr. Socks ran as a whole number or decimal value (seconds): "))
            if (travel_time < 0):
                print("Mr. Socks' travel time cannot be negative. Please enter a positive numerical value.")
                continue
        except ValueError:
            print("Only positive numerical values are valid. Please enter a valid value.")
            continue
        else:
            break
            
    final_position = float(initial_position + initial_velocity * travel_time + 0.5 * acceleration_rate * travel_time * travel_time)

    print("\nYou determine that Mr. Socks ran", final_position, "meters from home. What a kitty! Let's hope it was in a straight line!")

    retry_calculation = input("\nYou can let Mr. Socks out again, but you will need to help locate him. It's only fair, yes? Would you like Mr. Socks to escape again? (y/n): ")

    if(retry_calculation == "y"):
        print("\nOld Man Jenkins does NOT appreciate that, but it is with the utmost pleasure that I welcome you back to...")
        continue

    if(retry_calculation != "y"):
        print("\nI'll take that as a no. Probably the responsible thing to do. Thank you for your help! You're a hero!")
        do_calculation = False
```

---

**More links:**
- [Home](https://github.com/ultrasoftcore345/Personal-Practice/edit/main/README.md)
- [Challenge Rules](https://github.com/ultrasoftcore345/Personal-Practice/blob/main/Rules)
- [Extra Achievements](https://github.com/ultrasoftcore345/Personal-Practice/blob/main/Achievements.md)
- [Class Overviews](https://github.com/ultrasoftcore345/Personal-Practice/blob/main/Classes.md)
- [Helpful Links](https://github.com/ultrasoftcore345/Personal-Practice/blob/main/Links.md)
