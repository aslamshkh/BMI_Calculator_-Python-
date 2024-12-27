# BMI_Calculator_Python


## The Table Of Contents

- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools](#tools)
- [Calculation Steps](#calculation-steps)
- [Code Body](#code-body)


### Project Overview

A BMI Calculator (Body Mass Index) that allows users to input their "Weight" and "Height" to gain insight of their body BMI classification. 

The project is made through jupyter notebook using python language that uses Kilograms (weight) and Centemeters (height) as perameters to calculate.


### Data Source

The calculator format and BMI classification index is borrowed from an online [Source](https://www.calculator.net/bmi-calculator.html) with some changes. 


| Classification  |	BMI       | 
| :---: | :---: | 
| Severe Thinness | < 16	    | 
| Mild Thinness   | 17 - 18.5 | 
| Normal	        | 18.5 - 25	| 
| Overweight	    | 25 - 30   |  
| Obese       	  | 30 - 35   | 



### Tools

- Jupyter Notebook
- Python



### Calculation Steps


1) Used "Input" function to create variables allowing users to put their Weight & Height.
```python
weight = input("Please enter your weight: ")
height = input("Please enter your height: ")
```

2) Created a new variable converting height from **Centimeters to Meters** as per the formula.
```python
height_c = (height/100)
BMI = (weight) / (height_c ** 2)
```

3) Converted **String to Integer** to match with the user inputs.
```python
weight = int(input("Please enter you weight: "))
height = int(input("Please enter you height: "))
```

4) Added 2 more input variables to personalise.
```python
name = input("Please enter your name: ")
gender = input("Please enter your gender: ")
```

5) Used **If, Elif, & Else** statements to create the BMI classification results.
```python
if (BMI > 0):
    if (BMI < 16):
        print(name + ", You are severely thin.")
    elif (BMI < 18.5):
        print(name + ", You are thin.")
    elif (BMI < 25):
        print(name + ", You are average.")
    elif (BMI < 30):
        print(name + ", You are overweight.")
    elif (BMI < 35):
        ptint(name + ", You are obese.")
else:
    print("Please enter a valid input.")
```



### Code Body
![BMI Calculator](https://github.com/user-attachments/assets/4fb45ed2-8711-444c-86e7-494c3cb728e6)



### Limitations

I had to remove all the zero values from the budget and revenue columns because they would have affected the accuracy of the conclusion from the analysis. There are still a few outlier after being omitted/ However, even then we have seen a positive collaboration between budget and number of votes with revenue. 




