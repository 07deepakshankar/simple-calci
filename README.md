#program to make a simple calculator

#function which adds  two numbers
def add(x,y):
    return x+y

#function which subtracts two numbers
def sub(x,y):
    return x-y
    
#function which multiply two numbers
def multi(x,y):
    return x*y
    
#function which divide two numbers
def div(x,y):
    return x/y
    
print("Choose operation:")
print("1.Addition")
print("2.Subtraction")
print("3.Multiplication")
print("4.Division")

while True:
    
    #input from the user
    choice = input("Enter choice(1/2/3/4):")
    
    #verify the input is one of choices
    if choice in('1','2','3','4'):
        num1 = float(input("Enter first number:"))
        num2 = float(input("Enter second number:"))
        
        if(choice == '1'):
            print(num1,"+",num2,"=".add(num1,num2))
            
        elif(choice == '2'):
            print(num1,"-",num2,"=",sub(num1,num2))
            
        elif(choice == '3'):
            print(num1,"*",num2,"=",multi(num1,num2))
            
        elif(choice == '4'):
            print(num1,"/",num2,"=",div(num1,num2))
            
        #check if user wants another calculation
        #break the while loop if answer is no
        next_calculation = input("Let's do next calculation? (yes/no):")
        if next_calculation == "no":
            break
    else:
        print("Invalid Input")
          
