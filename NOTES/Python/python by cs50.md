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
###### WEEK - 1 : PROBLEM SET 1 Conditionals
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
- The `split()` function in Python breaks a string into smaller pieces, called "substrings," based on a specific separator. If you don't specify a separator, it will split the string by spaces.
- Meal time: In this we have to determine weather it is breakfast, lunch or dinner time.
```
def main():
	a = input("What is the time? ")
	time = convert(a)
	if 7 <= time <= 8:
		print("breakfast time")
	elif 12 <= time <= 13:
		print("lunch time")
	elif 18 <= time <= 19:
		print("dinner time")
def convert(time):
    hours, minutes = time.split(":")
    mins = float(minutes) / 60
    return float(hours) + mins


if __name__ == "__main__":
    main()
```
To solve the problem, we first need to take the time as input in the main function, typically in the format "hours: minutes". To process this input, we convert it into a decimal representation of time. For this purpose, we use a helper function named `convert`. Inside the `convert` function, we split the input string into hours and minutes using the `split` function, which separates the two components based on the colon ":". Once we have the hours and minutes, we calculate the decimal equivalent of the minutes by dividing them by 60. We then add this value to the hours to get the total time in decimal form. After computing the result, we return this decimal value to the main function. Finally, using conditional statements like `if-else`, we can easily solve the problem by performing any required comparisons or calculations based on the decimal time obtained. This approach ensures clarity and efficiency in handling time-related computations.

###### WEEK - 2: Loops Problem set 2
- camelCase: We need to convert camel case to snake case which is `snake_case`.
```
camel = input("camelCase: ")
snake = ''
for char in camel:
    if char.isupper():
        snake += "_" + char.lower()
    else:
        snake += char
print("snake_case: ", snake)
```
For this we took camel case input from the use and took an empty sting in snake. now using for loop we take characters in camel and checks with if condition weather it is upper or not. If upper then it prints like `suppose 'httpRequset' then it prints http_request`. So it basically divides the the part first then add `_` and adds the rest part in lower characters. If not upper it directly prints the camel case input. 

- Coke Machine: For this problem the amount is fixed which is 50 cents and there are 3 coins which are {25, 10, 5}. so we need to make the amount 0 by inserting coins.
```
def main():
	total = 0
	while True:
		coin = int(input("insert coin: "))
		if coin in {5,10,25}:
			total += coin
			print(f"Amount Due: {50 - total}")
			if total >= 50:
				change = total - 50
				print(f"Change owed: {change}")
				break
			else:
	            print(f"Amount Due: {50}")
main()
```
So, for this we took the initial total value as 0. Now we used while true to create a loop and gave input of coin. Now if coin are those 3 values then we replace total value with coin. Now we deduct the the amount and give amount due with print function. After this we too if function and checked weather total greater or equal to 50 which shows how much amo
unt is left over and if its 0 