# PYTHON
import sys
budget = 10
flavours = ['chocolate', 'vanilla', 'strawberry']
while budget >= 0:
    budget = int(input("please enter how much money you have"))
    selection = input("What flavour would you like? Chocolate, Vanilla or Strawberry ").lower()
    if selection == 'chocolate':
        print(f"here's your {flavours[0]} milkshake\n")
        budget -= 3
    elif selection == 'vanilla':
        print(f"here's your {flavours[1]} milkshake\n")
        budget -= 1
    elif selection == 'strawberry':
        budget -= 2
        print(f"here's your {flavours[2]} milkshake\n")
    else:
        print("See you next time, Sam!")
        sys.exit()
    if budget <= 0:
        print("You've had enough, you're barred...")
        sys.exit()
    
    print(f"your budget is £{budget}")
