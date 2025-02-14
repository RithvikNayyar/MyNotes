###### WEEK 0 - PROBLEM SET 0
- All caps to small
```
x = input("Hey How are you? Please Write in all caps. : ")
y = x.lower()
print(y)
## INPUT = I AM FINE  OUTPUT = i am fine
```
In the above problem we learn about how to make a upper case string to lower case. In python we have a in built function which helps to make the string lower. 
 str.Lower( ) : Converts all uppercase characters in a string to lowercase.
 
- Pause between the word
```
x = input("SUPP?? :")
y = x.replace(" ","...")
print(y)
```
In the above problem we need to replace space or " " with ". . ." so, we used a python in build function which is-
Str.Replace( ) : It replaces anything which you specify or Replaces occurrences of `old` substring with `new` substring in a string.

-  Changes to emoji. In this question we need to change emoji from ': )' to 😀and various other emoji faces.
```
x = input("")
y = x.replace(":)","🙂").replace(":(","🙁")
print(y)
```
For this we will approach with .replace( ) function. We will not use  ' emoji.Emojize ( ) ' function as they are in short form and for this function to work we anyways need to to use replace function. Basically, it makes the code even more lengthy. 

- Einstein famous problem e = mc^2
```
c = (90000000000000000)
m = int(input())
e = m*c
print(e)
```
For this we already got input from the user that c^2= 90000000000000000. We need to take input from the user for m and that's it.

- Tip calculator: Basic functionality of conversion of string to float.
```
def main():
    dollars = dollars_to_float(input("How much was the meal? "))
    percent = percent_to_float(input("What percentage would you like to tip? "))
    tip = dollars * percent
    print(f"Leave ${tip:.2f}")
def dollars_to_float(d):
    return float(d.replace("$", ""))
def percent_to_float(p):
    return float(p.replace("%", "")) / 100
if __name__ == "__main__":
    main()
```

WEEK 0 is Completed with this.
###### WEEK - 1 : 
- Deep thought: In this if the number 42 is written in number or Forty-Two or forty two they print yes and rest no.
```
i = input("").lower()
j = i.replace("-","").replace(" ","")
if j == '42' or j == 'fortytwo':
    print("yes")
else:
   print("no")
```
For this approach we use .replace( ) function to first to remove all the extra things like   '-' and spaces. Then use .lower( ) function to lower all the caps. Now we use if statement to say yes if y = 42 or y = fortytwo. That's it. 

- Home Federal Savings Bank: If the bank says hello then it is $0. If bank say anything that starts with h then $20 and if the bank says anything else then $100.
```
i = input("Greeting: ").lower().strip()
if "hello" in i:
    print("$0")
elif i[0] == 'h' :
    print("$20")
else:
    print("$100")
```
For this we initially take greetings from bank. Then we make it all in small letters and use strip to remove all the spaces from the string. Now we use if statement to complete the program.

- File extensions: In this we need to determine what application are we running in our system. Like .png or .jpg or .pdf or running application. 
```
i = input("File name: ").lower()
i = '.' + i.split('.')[-1]
if '.gif' in i:
    print("image/gif")
elif '.png' in i:
    print("image/png")
elif ".jpg" in i:
    print("image/jpeg")
elif ".jpeg" in i:
    print("image/jpeg")
elif ".pdf" in i:
    print("application/pdf")
elif ".zip" in i:
    print("application/zip")
elif ".txt" in i:
    print("text/plain")
else:
    print("application/octet-stream")
```
Firstly we take input from the user. Now we make it all lower just in case we got input like .Png soo to avoid those mistakes. Now we separate the input given by user from the last by using [-1], because the user may also give input which is like 'hello.txt.jpg' so to avoid this we use .strip( ) function. Now there is a problem that using strip function we need to add a '.' as the input is stripped from the dot. Now using if else we can complete the program.

- Math Interpreter: Basic math problem where we need to give output in float.
```
i, j, k= input("Expression : ").split()
i = float(i)
k = float(k)
if '+' in j:
    a = i + k
    print(a)
elif '-' in j:
    a = i - k
    print(a)
elif '*' in j:
    a = i * k
    print(a)
elif '/' in j:
    a = i / k
    print(a)
```
Firstly we take input from the user and use split function to remove all the spaces other wise we will encounter a issue of spaces where it says there are 5 inputs but there are actually 3. Now we convert i and k to float so that there values become if 5 then 5.0. Now by using basic if-else function we can solve this problem.

- Meal time: 