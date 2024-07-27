#Python Essentials II - 2.4.1.6 LAB A LED Display
# Multiple-purpose-LED-display
This program is to simulate LED display digitls/float, clock and date written by Fulian Qiu
# ' ' represents 0 and '#' represents 1 in real world LED display
print('This program is for mimic digital LED display')

num = input("Enter a number for LED display:")

#Define functions for digit segments

#Three

def th_3():
    print('###',end=' ')
       
#left-right

def lr_2():
    print('# #',end=' ')
    
#left one 

def lt_1():
    print('#  ',end=' ')
    
#right one

def rt_1():
    print('  #',end=' ')
    
def one_1():
    print('#',end=' ')
    
def zero_1():
    print(' ',end=' ')

def line():
    print('-',end=' ')
    
def time_1():
    print('*',end=' ')
    
#End of function defination
    
#Every digit composed of five lines or
#layers from top to bottom
    
for x in range(5):

    print()     
    
    for i in num:

        if x == 0:
            
        #display first line(row)

            if i == "1":
                one_1()
            if i == "2":
                th_3()
            if i == "3":
                th_3()
            if i == "4":
                lr_2()
            if i == "5":
                th_3()
            if i == "6":
                th_3()
            if i == "7":
                th_3()
            if i == "8":
                th_3()
            if i == "9":
                th_3()
            if i == "0":
                th_3()
            if i == ".":
                zero_1()
            if i == ":":
                zero_1()
            if i == "-":
                zero_1()  
        elif x == 1:
            
        #display second line(row)
            
            if i == "1":
                one_1()
            if i == "2":
                rt_1()
            if i == "3":
                rt_1()
            if i == "4":
                lr_2()
            if i == "5":
                lt_1()
            if i == "6":
                lt_1()
            if i == "7":
                rt_1()
            if i == "8":
                lr_2()
            if i == "9":
                lr_2()
            if i == "0":
                lr_2()
            if i == ".":
                zero_1()                
            if i == ":":
                time_1()
            if i == "-":
                zero_1()                      
        elif x == 2:
                
        #display third line(row)
            
            if i == "1":
                one_1()
            if i == "2":
                th_3()
            if i == "3":
                th_3()
            if i == "4":
                th_3()
            if i == "5":
                th_3()
            if i == "6":
                th_3()
            if i == "7":
                rt_1()
            if i == "8":
                th_3()
            if i == "9":
                th_3()
            if i == "0":
                lr_2()
            if i == ".":
                zero_1()
            if i == ":":
                zero_1()
            if i == "-":
                line()
        elif x == 3:

        #if display fourth line(row)
            
            if i == "1":
                one_1() 
            if i == "2":
                lt_1()
            if i == "3":
                rt_1()
            if i == "4":
                rt_1()
            if i == "5":
                rt_1()
            if i == "6":
                lr_2()
            if i == "7":
                rt_1()
            if i == "8":
                lr_2()
            if i == "9":
                rt_1()
            if i == "0":
                lr_2()
            if i == ".":
                zero_1()
            if i == ":":
                time_1()
            if i == "-":
                zero_1()  
        else:
            
        #display five line(row)
            
            if i == "1":
                one_1() 
            if i == "2":
                th_3()
            if i == "3":
                th_3()
            if i == "4":
                rt_1()
            if i == "5":
                th_3()
            if i == "6":
                th_3()
            if i == "7":
                rt_1()
            if i == "8":
                th_3()
            if i == "9":
                th_3()
            if i == "0":
                th_3()                
            if i == ".":
                time_1()
            if i == ":":
                zero_1()
            if i == "-":
                zero_1()  
#End of digit display
