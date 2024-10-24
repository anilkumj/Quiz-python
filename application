class restaurant:
    def __init__(self):
        self.restaurant_name = "Welcome to Food on Wheels"
        self.total_bill = 0  

    def item_list(self):
        while True:
            print("\nMenu Options:")
            print("1. Main Course")
            print("2. Vegetarian Items")
            print("3. Starters")
            print("4. Desserts")
            print("5. Pay Bill")
            print("6. Exit")
            try:
                n = int(input("Select an option: "))
            except ValueError:
                print("Please enter a valid number.")
                continue

            if n == 1:
                print("\nMain Course")
                print("items                : Half : Full")
                print("1. Chicken Dum Biryani  : 139  : 259")
                print("2. Chicken Fry Biryani  : 129  : 249")
                print("3. Mutton Dum Biryani   : 159  : 289")
                print("4. Fish Fry Biryani     : 169  : 299")
                print("5. Prawns Dum Biryani   : 179  : 309")
                print("--------------------------------------------------------")
                try:
                    n1 = int(input("Select the Non-veg item you want to order: "))
                    prices_main = {1: 139, 2: 129, 3: 159, 4: 169, 5: 179}
                    prices_main1 = {1: 259, 2: 249, 3: 289, 4: 299, 5: 309}
                    if n1 in prices_main or n1 in prices_main1:
                        self.total_bill += prices_main[n1]
                        print(f"Added to bill: {n1}. Current Total Bill: {self.total_bill}")
                    else:
                        print("Invalid selection.")
                except ValueError:
                    print("Please enter a valid number.")
                print("--------------------------------------------------------")

            elif n == 2:
                print("\nVegetarian Items")
                print("1. Veg Biryani  : 119  : 229")
                print("2. Egg Biryani  : 99   : 149")
                print("3. Paneer Dum Biryani  : 159  : 249")
                print("4. Egg Fried Rice      : 70   : 150")
                print("5. Rice with Dal and Chapathi : 79 : 110")
                print("6. Rice with Two Curries, Chapati, One Papad : 80 : 120")
                print("--------------------------------------------------------")
                try:
                    n2 = int(input("Select the veg item you want to order: "))
                    prices_veg = {1: 119, 2: 99, 3: 159, 4: 70, 5: 79, 6: 80}
                    if n2 in prices_veg:
                        self.total_bill += prices_veg[n2]
                        print(f"Added to bill: {n2}. Current Total Bill: {self.total_bill}")
                    else:
                        print("Invalid selection.")
                except ValueError:
                    print("Please enter a valid number.")
                print("--------------------------------------------------------")

            elif n == 3:
                print("\nStarters")
                print("1. Chicken Fry         : 80")
                print("2. Chicken Liver       : 90")
                print("3. Chicken Roast       : 80")
                print("4. Chicken Manchurian  : 100")
                print("5. Chicken Lasaguniya  : 110")
                print("6. Paneer Tikka        : 70")
                print("7. Paneer Roast        : 80")
                print("8. Mushroom Tikka      : 90")
                print("--------------------------------------------------------")
                try:
                    n3 = int(input("Select the starter you want to order: "))
                    prices_starters = {1: 80, 2: 90, 3: 80, 4: 100, 5: 110, 6: 70, 7: 80, 8: 90}
                    if n3 in prices_starters:
                        self.total_bill += prices_starters[n3]
                        print(f"Added to bill: {n3}. Current Total Bill: {self.total_bill}")
                    else:
                        print("Invalid selection.")
                except ValueError:
                    print("Please enter a valid number.")
                print("--------------------------------------------------------")

            elif n == 4:
                print("\nDesserts")
                print("1. Apple Pie               : 110")
                print("2. Tiramisu                : 120")
                print("3. Cheese Cake             : 130")
                print("4. Brownie Cake            : 110")
                print("5. Chocolate Cake          : 110")
                print("6. Ice Cream with Two Flavors : 80")
                print("7. Cold Drinks             : as per MRP")
                print("-------------------------------------------------------")
                try:
                    n4 = int(input("Select the dessert you want to order: "))
                    prices_desserts = {1: 110, 2: 120, 3: 130, 4: 110, 5: 110, 6: 80, 7: 0}
                    if n4 in prices_desserts:
                        if n4 == 7:
                            print("Please pay as per MRP for Cold Drinks.")
                        else:
                            self.total_bill += prices_desserts[n4]
                            print(f"Added to bill: {n4}. Current Total Bill: {self.total_bill}")
                    else:
                        print("Invalid selection.")
                except ValueError:
                    print("Please enter a valid number.")
                print("-------------------------------------------------------")

            elif n == 5:
                print("Pay Bill")
                print(f"Your total bill is: {self.total_bill}")
                print("---------------------------------------------------------")
                n9 = input("Enter the payment method (PhonePe, GPay, Paytm, Cash): ").lower()
                if n9 in ["phonepe", "gpay", "paytm"]:
                    print(f"Processing payment of {self.total_bill} via {n9.capitalize()}...")
                    print(f"{n9.capitalize()} payment accepted.")
                elif n9 == "cash":
                    print(f"Processing cash payment of {self.total_bill}...")
                    print("Cash payment accepted.")
                else:
                    print("Invalid payment method selected.")
                print("Thank you so much, visit again!")
                break  

            elif n == 6:
                print("Exit")
                print("Thank you so much, visit again!")
                break  

            else:
                print("Invalid option, please try again.")

# Instantiate and run the restaurant ordering system
a = restaurant()
print(a.restaurant_name)
a.item_list()
