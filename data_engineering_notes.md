#Data Processing with Python<br>

First Session:🙌<br>

print("your BMI is:",{BMI})<br>
print(f"your BMI is: {BMI}")<br>
print('your BMI is:' + str(BMI))<br>
print("your BMI", BMI, sep= ":")<br>

cleaning console ---> ctrl + L

x1 = True
X2 = False
x1 + x2 = 0 + 1 = 1

str1 + str2 = Concat

Data type is very effective on the result.

#Defensive Programming : For preventing Errors

#Complex Types: List[], Dict{}
list works with indexes
dict works with keys

#Slicing rules on List(names[a, b, c])
List[start:End] ----> End is exclusive
del variable, del names[0]-------> Delete a variable
['Maryam'] + names

Dictionary{Key:Value}
mydict = dict(zip(keys,values))

mutable(changeable): List, Dict values, Set
immutable(unchangeable): Dict keys, tuples, floats, ints, strs,...

Functional Programming(FP) / Object_Oriented Programming (OOP)

Piping/Chaining
Piping: Cat file.txt | grep "Keyword" | Sort
Chaining: # Chaining inbuilt functions
result = text.strip().upper().replace("WORLD", "FRIEND")

Funtions:(indentation is very important)
def FuncName(arg):
    return(expr)

Sometimes arg is not needed, 
e.g: # Current date and time
now = datetime.now()

explanation about Functions:
help(sum)
?sum
SPYDER---> tools-->preferences--->Help--> active all sections

a---> z : z has bigger Ascii code for sorting (Ascci code of Capital letter is bigger than small letter A > a)
len(lst) number of elements in mentioned list 
sorted(lst, reverse=True)

using cheat sheet is very important

String Methods:
'ali'.capitilize
'ali'.upper()
'Ali'.lower()
'maryam hosseini'.count('a')
'maryam hosseini'.count('gh')
'maryam hosseini'.index('i')
'maryam hosseini'.index('i',3) ---> from third element afterward
'maryam hosseini'.split() ---> split by distance
'maryam hosseini'.split('i') ---> split by i
list('maryam hosseini') break down into each letter

Iterable / Iterator
# gready methods
lst = [1,2,1,3,1,4]
lst.index
lst.count(1)
lst.append(1)
lst.remove(1)
lst.reverse()


lst.pop()
lst.pop(index)

# Dictionary : pair of key, value (key,value)
DictName.keys()---> key
DictName.values()---> value
DictName.items() ---> (key,value)

DictName[key] ---> value
for slicing a dictionary by Index, it should be converted to a list
a dictinary works by keys and a list works by indexes

list(DictName.keys())[0]
list(DictName.items())[0][0]

# adding new item to a dict
DictName[key]=value 
# deleting an item from a dict
del DictName[key]
DictName[key].pop(key)
# changing an item in a dict
DictName[key]= new value 

*When order is important ,we use **lists** and when finding values based on keys is important, **Dictionaries** should be considered.*
*NOSQL logic is using several nested Dictionaries*

Example of a nested dictionary:
italy = {'capital': 'rome', 'population': 59.83 }
spain = {'capital': 'madrid', 'population': 46.77 }
france = {'capital': 'paris', 'population': 66.03 }
germany= {'capital': 'berlin', 'population': 80.62 }
norway= {'capital': 'oslo', 'population': 5.084 }
europe = {'italy': italy, 'spain': spain, 'france': france, 'germany': germany, 'norway': norway}
europe
europe['france']
result = europe['france']
result
result['capital']
europe['france']
europe['france']['capital']

# in applications
'Ali' in 'alireza'   ---> False
'Ali'.lower() in 'alireza' ---> True
lst = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
5 in lst   ---> True
11 in lst  ---> False
lst2 = ['ali', 'sadeghi']
'ali' in lst2  ---> True
'akbar' in lst2  ---> False
familyDict
familyDict['father'] = 175
familyDict
175 in familyDict  ---> True
'father' in familyDict  ---> False
'son2' in familyDict  ---> True
'180' in familyDict  ---> False
familyDict.values()  
170 in familyDict.values()  ---> True

import numpy
heights = [184, 175]
weights = [76, 66]
BMI = weight/height ** 2
BMI = weights/heights ** 2
weights[0]/heights[0] ** 2
weights[1]/heights[1] ** 2
weights[0]/(heights[0]/100) ** 2
weights[1]/(heights[1]/100) ** 2
BMI = [bmi1, bmi2]
bmi1 = weights[0]/(heights[0]/100) ** 2
bmi2 = weights[1]/(heights[1]/100) ** 2
BMI = [bmi1, bmi2]
BMI
def multiply(lst1, lst2):
    y = 0
    lst = []
        for element1 in lst1:
            for element2 in lst2:
                multiply = element1 * element2
                lst.append(multiply)
                y += 1
                break
    return lst
def multiply(lst1, lst2):
    y = 0
    lst = []
    for element1 in lst1:
        for element2 in lst2:
            multiply = element1 * element2
            lst.append(multiply)
            y += 1
            break
    return lst
multiply(num1, num2)
num1 = [1, 2, 3]
num2 = [1, 2, 3]
multiply(num1, num2)
def multiply(lst1, lst2):
    y = 0
    lst = []
    for element1 in lst1:
        for element2 in lst2[y:]:
            multiply = element1 * element2
            lst.append(multiply)
            y += 1
            break
    return lst
multiply(num1, num2)
npNum1 = np.array(num1)
import numpy as np
npNum1 = np.array(
npNum1 = np.array(num1)
npNum2 = np.array(num2)
npNum1 * npNum2
np.random.rand(10)
v1 = np.random.rand(1000000)
v2 = np.random.rand(1000000)
v1 = np.random.rand(100000)
v2 = np.random.rand(100000)
# Magic commands on IPYTHON
%time v1 * v2
v1 = np.random.rand(1000000)
v2 = np.random.rand(1000000)
%time v1 * v2
v1 = np.random.rand(100000)
v2 = np.random.rand(100000)
%time multiply(v1,v2)
%time a = multiply(v1,v2)
v1 = np.random.rand(1000000)
v2 = np.random.rand(1000000)
%time v1 * v2
npHeights = np.array(heights)
npWeights = np.array(weights)
BMI = npWeights/npHeights ** 2
BMI
BMI = npWeights/(npHeights/100) ** 2
BMI
BMI[0]
BMI[1]
npHeights[0]
type(npHeights)
range(10)
type(range(10))
list(range(10))
list(range(10, 20))
list(range(10, 20, 2))
np.arange(10)
np.arange(10, 20)
np.arange(10, 20, 2)
np.arange(12)
lst = [[0, 1, 2, 3, 4, 5], [6, 7, 8, 9, 10, 11]]
np.array(lst)
np.arange(12)
np.arange(12).reshape(2, 6)
np2d = np.arange(12).reshape(2, 6)
np2d
np2d.reshape(-1,)  *reshape 2 dimension into one dimension*
np2d.reshape(3, 4)
np2d = np2d.reshape(3, 4)
np2d
# Slicing in NUMPY
np2d[1]
np2d[1][2]
np2d[1, 2]
np2d
np2d[2]
np2d[2][:]
np2d[2, :]
np2d
np2d[:,2]
%clear
np2d
np2d.transpose()
np2d.T
%clear
weight
height
npWeight = np.array(weight)
npHeight = np.array(height)
BMI = npWeight / npHeight ** 2
BMI
BMI = npWeight * 0.453592 / (npHeight * 0.0254) ** 2
BMI
np.array([weight, height])
np.array([weight, height]).T
np.array([weight, height]).T * np.array([0.453592, 0.0254])
info = np.array([weight, height]).T * np.array([0.453592, 0.0254])
info [:, 1] / info[:, 2] ** 2
info [:, 0] / info[:, 1] ** 2
2 > 3
2 < 5
[1, 2, 3, 4, 5, 6]
[1, 2, 3, 4, 5, 6] > 3
# recycling
# broadcasting
np.array([1, 2, 3, 4, 5, 6])
np.array([1, 2, 3, 4, 5, 6]) > 3
np.array([1, 2, 3, 4, 5, 6]) > np.array([3, 3, 3, 3, 3, 3])
BMI
BMI < 22
len(BMI)
BMI[BMI < 22]
np.array([1, 2, 3, 4, 5, 6]) > 3
lst = np.array([1, 2, 3, 4, 5, 6])
lst > 3
lst[lst > 3]
info
info.ndim
info.shape
info.size
len(info)
np.array([weight, height])
npWeight
npHeight
np.column_stack((npWeight, npHeight))
np.row_stack((npWeight, npHeight))
nums = np.arange(200)
nums
np.mean(nums)
nums.mean()
np.std(nums)
nums.std()
np.abs([-12, 2, 5, -3])
[-12, 2, 5, -3].abs()
np.array([-12, 2, 5, -3]).abs()
np.max(nums)
nums.max()
np.median(nums)
nums.median()
%clear
height
weight
age
position
num1
lst1
v1
v2
v1 * v2
np.dot(v1, v2)
a1 = np.array([1, 2, 3, 4]).reshape(2, 2)
a1
a2 = np.array([1, 2, 3, 4]).reshape(2, 2)
np.cross(a1, a2)
np.matrix()
np.matrix(range(100))
np.matrix(range(100)).reshape(4, 25)

# Pandas
import pandas as pd
names = ['ali', 'hassan', 'meysam']
family = ['sadeghi aghili', 'eskandari', 'kermani']
age = [36, 36, 41]
major = ['Automation', 'Programming', 'Computer Science']
info = {'name':names, 'family': family, 'major': major, 'age': age}
info
pd.DataFrame(info)
infoDF = pd.DataFrame(info)
infoDF
type(infoDF)
infoDF.columns
infoDF.index
infoDF.columns[2]
infoDF.columns[2] = 'field'
infoDF.index
infoDF.index[0] = 'a'
infoDF.index = ['a', 'b', 'c']
infoDF
countries = ['United States', 'Australia', 'Japan','India', 'Russia', 'Morocco', 'Egypt']
drivesRight = [True, False, False, False, True, True, True]
carsPerCapita = [809, 731, 588, 18, 200, 70, 45]
carsInfo = pd.DataFrame({'country': countries, 'dr': drivesRight, 'cpc': carsPerCapita})
carsInfo
carsInfo.index = ['USA', 'AUS', 'JAP', 'IND', 'RUS', 'MOR', 'EGP']
carsInfo
input()
input('please enter your name:' )
name = input('please enter your name:' )
name
age = input('please enter your age: ' )
age
int(age)














