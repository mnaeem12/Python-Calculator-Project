# Python-Calculator-Project
# This repository for Python's Projects
print ('*********Simple Calculator*******')
operations =('+', '-', '*', '/')
print ('Enter one of operations below ')
f=0
while True:
    operation = input(' +: Sumation\n -: Subtraction\n *: Multiplication\n \\: Devision\n :>>')
    f=0
    if operation in ('+', '-', '*', '/'):
        while True:
            try:
                x=float(input('Enter the first number :>'))
                y=float(input('Enter the second Number:>'))
                break 
            except ValueError:
                print ('\nplease Ener valid Numbers ')
                
    else:
        print ('\nplease Ener valid operation')       
        
    if operation =='+':
        z=x+y
        print (x, operation, y, '=',z)
        f=1
    elif operation== '-':
        z=x-y
        print (x, operation, y, '=',z)
        f=1
    elif operation== '*':
        z=x*y
        print (x, operation, y, '=',z)
        f=1
    elif operation== '/':
        z=x/y
        print (x, operation, y, '=',z)
        f=1
    if f==1:
        if(input('\npress "y" for new operation \npress any key to exit\n:>>').lower()=='y'):
            print ('Enter one if operations below ')
            continue
        else:
            print ('Thank you')
            break    
   
