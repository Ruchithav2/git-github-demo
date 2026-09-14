# Python-Projects

## Project 1: Random Number Guessing Game

### Description: This is a number guessing game where the player has to guess a randomly selected number between 1 and 100 within a limited number of attempts based on the chosen difficulty level. After each round, the player can choose to play again or exit the game.

### Algorithm: 
1. Generate a random number between 1 and 100.
2. Ask the player to choose a difficulty level:
     * EASY → 10 attempts
     * HARD → 5 attempts
3. Repeat until attempts run out or the player guesses correctly:
   * Show attempts remaining.
   * Prompt the player to enter a guess.
   * Compare the guess with the secret number:
       * If equal → Print the success message, end round.
       * If greater → Prompt the player to guess lower number.
       * If smaller → Prompt the player to guess higher number.
   * Decrement attempts.
4. If attempts reach 0 without a correct guess → Reveal the secret number and print failure message.
5. Ask the player if they want to play again:
    * If yes → Restart from step 2.
    * If no → Exit with a goodbye message.

![output](guess_no_output.png)


## Project 2: Vending Machine

### Description: A Python-based vending machine that allows customers to select and purchase multiple items.The system checks product availability and stock before adding items to the cart.It accepts valid coins, calculates the total amount, and returns the appropriate change.After successful payment, the machine dispenses the items and updates the remaining stock.

### Algorithm:
1. Display Menu
    * Display all available products.
    * Display the price and current stock of each product.
2. Select Product
    * Ask the customer to select a product.
    * Check whether the selected product exists.
    * If the product does not exist, display an error message and ask again.
3. Check Stock
    * Check whether the selected product is available.
    * If stock is zero, display "Out of Stock" and return to the menu.
    * Otherwise, continue.
4. Select Quantity
    * Ask the customer for the required quantity.
    * Check whether the requested quantity is valid.
    * Compare the requested quantity with the available stock.
    * If sufficient stock is unavailable, notify the customer.
    * Otherwise, add the selected product and quantity to the cart.
5. Continue Shopping
    * Ask the customer whether they want to purchase another product.
    * If Yes, display the menu again and repeat the selection process.
    * If No, proceed to billing.
6. Calculate Bill
    * Calculate the cost of each product:
   - Item Cost = Price × Quantity
    * Add the cost of all selected products.
    * Display the final bill.
7. Accept Coins
    * Display the accepted coin denominations:
       * ₹1, ₹2, ₹5, ₹10, ₹20, ₹50
    * Ask the customer to insert coins.
    * Check whether each inserted coin is valid.
    * If invalid, reject the coin and ask again.
    * Continue accepting coins until the inserted amount is equal to or greater than the total bill.
8. Calculate Change
    * Calculate:
        * Change = Total Amount Inserted − Total Bill
    * If the change is greater than zero, return the change to the customer.
    * If the amounts are equal, no change is returned.
9. Dispense Products
    * Dispense each product in the cart.
    * Reduce the stock according to the quantity purchased.
10. Complete Transaction
    * Display a successful payment message.
    * Display the dispensed products.
    * Display the change, if applicable.
    * Display a thank-you message.
11. End
    * End the current transaction.

![output](vending-op1.png)
![output](vending-op2.png)















