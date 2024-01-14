# Python Lab 2.1: Conditionals 
In `lab2_1.py` in the text editor at top-right, write a few python commands to:

1. Ask the user to type their score in a test and store it in a variable
2. Test if the score entered by the user falls within the valid range from 0 to 100. If not display `Invalid score`.
3. If the user enters character/s instead of a number display `Wrong input`.
4. Using the following table to find and display the letter grade of the user score.

![Image of ranges](ranges.png)

Click next to see the flowchart of this algorithm...


## Flowchart v1 
This Flowchart represents the logic of this program... 
[![Flowchart](https://mermaid.ink/img/pako:eNpd0l1vgjAUBuC_0pzdzEQTdrMPZkzkSwiiF3ql5aKBMkmAulK2LMT_vgLaULiBc_r2OSVpCwlLKZiQFew3uRAu0NHBFZLP-vlcC9mIZ2ixWCHrjMGtBOXokDBOMcRDzJKr6Mgb2qfsFkPdraMlMhDjqC9WL4aB4TZssLUNrmSfvhsmPoPqhxR5OvBDSw1x--xpBHikqAfBax8DXw10n-FpMzZqhjdxN2PX011fuW_K9TU3UK4zcYOx6-tuqNx35Yaau1WuPXG3YzfU3Ui5H8qNNHenXGviRjq1V8H1JLgbH2A_Lk7ddWHXeNaXuOpeMIeS8pLkqbxhbdfBIC60lLfHlJ8pzUhTCAy4usloc02JoG6aC8bBzLrTzIE0gh3-qgRMIX_jEXJy8sVJeU_d_gExhcnT)](https://mermaid.live/edit#pako:eNpd0l1vgjAUBuC_0pzdzEQTdrMPZkzkSwiiF3ql5aKBMkmAulK2LMT_vgLaULiBc_r2OSVpCwlLKZiQFew3uRAu0NHBFZLP-vlcC9mIZ2ixWCHrjMGtBOXokDBOMcRDzJKr6Mgb2qfsFkPdraMlMhDjqC9WL4aB4TZssLUNrmSfvhsmPoPqhxR5OvBDSw1x--xpBHikqAfBax8DXw10n-FpMzZqhjdxN2PX011fuW_K9TU3UK4zcYOx6-tuqNx35Yaau1WuPXG3YzfU3Ui5H8qNNHenXGviRjq1V8H1JLgbH2A_Lk7ddWHXeNaXuOpeMIeS8pLkqbxhbdfBIC60lLfHlJ8pzUhTCAy4usloc02JoG6aC8bBzLrTzIE0gh3-qgRMIX_jEXJy8sVJeU_d_gExhcnT)


Remember that you can reverse the checks and still have a valid program!
So click next to see a reverse flowchart...



## Reverse Flowchart

[![ReverseFlowchart](https://mermaid.ink/img/pako:eNpd0s9vgjAUB_B_pXm7zEQTd9gvXEgEQQiiBz1pOTRQJglQV8qWhfC_r4BrKFzgvX77eSVpAzFLKBiQ5uwnvhIu0GmDSySf9eOlErIRzdBiYSLrgsEpBeXoGDNOMURDzJKr6MRr2qfsBkPVraMPtESMo74wn5ZLDO2wwdY2OJJ9-KqZWPnlN8mzZOCHlhri9NnzCHBJXg2C2wwDTfT2ju4zXG3GVs1YT9zt2HV111Puq3I9zfWVa01cf-x6uhso90W5gebulGtP3N3YDXQ3VO6zckPN3St3M3FDnTqooDsJ7scHOIyLc3dd2C2a9SUuuxfMoaC8IFkib1jTdTCIKy3k7THkZ0JTUucCAy5bGa1vCRHUSTLBOBhpd5o5kFqw428ZgyHkb_yHNhn55KS4p9o_Z9TJ-w)](https://mermaid.live/edit#pako:eNpd0s9vgjAUB_B_pXm7zEQTd9gvXEgEQQiiBz1pOTRQJglQV8qWhfC_r4BrKFzgvX77eSVpAzFLKBiQ5uwnvhIu0GmDSySf9eOlErIRzdBiYSLrgsEpBeXoGDNOMURDzJKr6MRr2qfsBkPVraMPtESMo74wn5ZLDO2wwdY2OJJ9-KqZWPnlN8mzZOCHlhri9NnzCHBJXg2C2wwDTfT2ju4zXG3GVs1YT9zt2HV111Puq3I9zfWVa01cf-x6uhso90W5gebulGtP3N3YDXQ3VO6zckPN3St3M3FDnTqooDsJ7scHOIyLc3dd2C2a9SUuuxfMoaC8IFkib1jTdTCIKy3k7THkZ0JTUucCAy5bGa1vCRHUSTLBOBhpd5o5kFqw428ZgyHkb_yHNhn55KS4p9o_Z9TJ-w)


Now, click next to start coding...



First ask the user to type a score
and validate the range

<details> 
<summary>
Hint 1 : Validate range  
</summary>


```
if score < 0 or score > 100 :
    print('Invalid score')`
```
</details>

What is the user types a letter instead of a number? 

<details> 
<summary>
Hint 2 : Invalid Input  
</summary>

use a try/except block after reading the score 
which will include the conversion to a floating point number...
and exit the program if the input is invalid.

```
try:
    score = float(score)
except:
    print('Wrong input')
    quit()
```

</details>

Now complete the if statement...

<details> 
<summary>
Hint 3 : Finding the letter grade 
</summary>


```
if score < 0 or score > 100:
    print('Invalid score')
elif score < 60: 
    print('F')
elif score < 70:
    print('D')
elif score < 80:
    print('C')
elif score < 90:
    print('B')
else:
    print('A')

```

</details>




Keep in mind that the sample solution is not the only solution. 
There are different ways to reach to the same result...


<details> 
<summary>
Solution : Putting it all together...
</summary>

```
try:
    score = float(score)
except:
    print('Wrong input')
    quit()

if score < 0 or score > 100:
    print('Invalid score')
elif score < 60: 
    print('F')
elif score < 70:
    print('D')
elif score < 80:
    print('C')
elif score < 90:
    print('B')
else:
    print('A')
```

</details>


## Execute your program 

Remember in order to execute your code you type in the terminal:
```
python lab2_1.py
```

Use the following test data to make sure your program produces correct resutls.

### TEST 1:

Enter your score: 35
F

### TEST 2:

Enter your score: 102
Invalid score

### TEST 3:

Enter your score: 60
D


### Check Your Code

Execute the below to evaluate the correctness of your code using `check50`, but be sure to test it yourself using:


- [x] a number out of the valid range
- [x] a character or word as input
- [x] a number below 60
- [x] a number in every possible range :tada:


```
check50 mkotsovoulou/ods6001a/main/labs/lab2_1
```

Execute the below to evaluate the style of your code using `style50`.

```
style50 lab2_1.py
```



## Submit your code

Execute the command below, logging in with your `GitHub username` and `Personal Access Token` when prompted. For security, you'll see asterisks (`*`) instead of the actual characters in your token. 

If you do not have generated a Personal Access ToKen follow the instructions: 
https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token

```
submit50 mkotsovoulou/ods6001a/main/labs/lab2_1
```

You can re-submit your solution as many times as you want.
When you are happy with your solution, download the code and upload it to Canvas.

![Image of download](download.png)

# Done!
:tada:
