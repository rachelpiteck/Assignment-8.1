# Assignment-8.1
#CIS245 Assignment 8.1, Rachel Moreira

class bankaccount:
    accountnumber1 = 12345
    accountnumber2 = 67890
    balance = 100, 25

    def withdrawal():
        wd = input(print("Please enter amount to withdraw: $"))
    def deposit():
        dep = input(print("Please enter deposit ammount: $"))
    def getBalance():
        bal = balance+dep-wd
        print("Your balance is :$ ", bal)

    class checking(bankaccount):
        fees = 5
        min_balance = 50

        def deductFees():
            if wd > balance:
                balance = balance-fees
            else:
                balance = balance
        def checkMinimumBalance():
            if balance == min_balance:
                print("Your balance is at its minimum. $", min_balance)
        
    class savings(bankaccount):
        interestRate = .02
        def addInterest():
            savingsbalance = 100
            i=1
            while(i<=12):
                savingsbalance +=savingsbalance *.02
                print("Your savings account balane is $", savingsbalance)
            

