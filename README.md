import random

def endless_journey():
    print("Welcome to the endless journey!")
    print("You will continue your journey until you decide to exit.")

    while True:
        event = random.randint(1, 3)

        if event == 1:
            print("You stumbled upon an ancient ruin.")
        elif event == 2:
            print("Your path crosses a mountain range.")
        elif event == 3:
            print("An unexpected obstacle appears on your way.")

        response = input("Continue the journey? (yes/no): ").lower()
        if response != 'yes':
            break

    print("Thank you for playing! Come back to your next endless journey.")

# Start the game
endless_journey()
