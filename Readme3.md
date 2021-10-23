# Information Technology 1040

Information Technology 1040 is a class introducing students to problem solving methods and programming concepts, providing experience in desinging, developing, implementing and testing programs. This course is based around Python and its platforms. After this course the student should have a basic understanding of how Python works and how to apply it to a variety of different situations and settings. 

### The following topics are covered in this course:

* Elements of a computer.
* Purpose of programming and programming languages.
* Types of programming languages and where Python fits.
* Problems that programming languages can solve.
* Analyzing problems and designing solutions.
* Program architecture and code organization.
* Installing and configuring Python and Python IDLE.
* Representing information digitally.
* Variables and data types.
* Decision structures and Boolean logic.
* Repetition structures.
* Writing and using functions.
* Working with strings.
* Using Lists and tuples.
* Using dictionaries and sets.
* Mathematical expressions and precision.
* File input and output.
* User input and output.
* Parsing data.
* Exception handling.
* Fundamental object-oriented concepts.

Go Back to [Main Page](https://github.com/corbyt32/corbyt32/blob/main/README.md)
#### Here is an example of code that estimates how much paint a person will need for a project _**Cylinder Coatings Estimator**_:
import math

area_per_pint = 400/8

while(True):
    radius = float(input("Enter radius of cylinder : "))
    height = float(input("Enter height of cylinder : "))
    cost_per_pint = float(input("Enter cost per pint of coating : "))
    
    if (radius < 0 or height < 0 or cost_per_pint < 0):
        print("Invalid Input")
        continue
    
    area = (2 * math.pi * radius) * (height + radius)
    
    total_pints = math.ceil(area/area_per_pint)
    
    total_cost = total_pints * cost_per_pint
    
    print("Total Cost :$", round(total_cost,2))
    print("Total Pints :", total_pints)
    
    another_calc = input("Want to do another calculation (Y/N): ")
    
    if another_calc.upper() == 'Y':
        continue
    else:
        break
