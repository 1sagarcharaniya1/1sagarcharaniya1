<!-- a Function to check if year number is a leap year. -->

def leapyear(year):
    if (year % 4) == 0:
        if (year % 100) == 0:
            if (year % 400) == 0:
                return True
            else:
                return False
        else:
            return True
    else:
        return False

year = int(input("enter valid year: "))             

if(leapyear(year)):
    print(year,"is leap year")
else:
    print(year,"is not a leap year")
