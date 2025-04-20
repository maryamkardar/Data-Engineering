#Data Processing with Python<br>

First Session:🙌<br>

print("your BMI is:",{BMI})<br>
print(f"your BMI is: {BMI}")<br>
print('your BMI is:' + str(BMI))<br>
print("your BMI", BMI, sep= ":")<br>

cleaning console ---> ctrl + L<br>

x1 = True<br>
X2 = False<br>
x1 + x2 = 0 + 1 = 1<br>

str1 + str2 = Concat<br>

Data type is very effective on the result.<br>

#Defensive Programming : For preventing Errors<br>

#Complex Types: List[], Dict{}<br>
list works with indexes<br>
dict works with keys<br>

#Slicing rules on List(names[a, b, c])<br>
List[start:End] ----> End is exclusive<br>
del variable, del names[0]-------> Delete a variable<br>
['Maryam'] + names<br>

Dictionary{Key:Value}<br>
mydict = dict(zip(keys,values))<br>

mutable(changeable): List, Dict values, Set<br>
immutable(unchangeable): Dict keys, tuples, floats, ints, strs,...<br>

Functional Programming(FP) / Object_Oriented Programming (OOP)<br>

*Piping/Chaining*<br>
Piping: Cat file.txt | grep "Keyword" | Sort<br>
Chaining: # Chaining inbuilt functions<br>
result = text.strip().upper().replace("WORLD", "FRIEND")<br>

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
import pandas as pd <br>
names = ['ali', 'hassan', 'meysam']<br>
family = ['sadeghi aghili', 'eskandari', 'kermani']<br>
age = [36, 36, 41]<br>
major = ['Automation', 'Programming', 'Computer Science']<br>
info = {'name':names, 'family': family, 'major': major, 'age': age}<br>
info<br>
pd.DataFrame(info)<br>
infoDF = pd.DataFrame(info)<br>
infoDF<br>
type(infoDF)<br>
infoDF.columns<br>
infoDF.index<br>
infoDF.columns[2]<br>
infoDF.columns[2] = 'field'<br>
infoDF.index<br>
infoDF.index[0] = 'a'<br>
infoDF.index = ['a', 'b', 'c']<br>
infoDF<br>
countries = ['United States', 'Australia', 'Japan','India', 'Russia', 'Morocco', 'Egypt']<br>
drivesRight = [True, False, False, False, True, True, True]<br>
carsPerCapita = [809, 731, 588, 18, 200, 70, 45]<br>
carsInfo = pd.DataFrame({'country': countries, 'dr': drivesRight, 'cpc': carsPerCapita})<br>
carsInfo<br>
carsInfo.index = ['USA', 'AUS', 'JAP', 'IND', 'RUS', 'MOR', 'EGP']<br>
carsInfo<br>
input()<br>
input('please enter your name:' )<br>
name = input('please enter your name:' )<br>
name<br>
age = input('please enter your age: ' )<br>
age<br>
int(age)<br>

## ---(Thu Oct 31 13:59:32 2024)---
import pandas as pd<br>
pd.read_csv('H:\Work\Python\Examples\1-basics\teachers.csv')<br>
pd.read_csv('H:\\Work\\Python\\Examples\\1-basics\\teachers.csv')<br>
pd.read_csv('H:/Work/Python/Examples/1-basics/teachers.csv')<br>
pd.read_csv(r'H:\Work\Python\Examples\1-basics\teachers.csv') # raw text<br>
path = input()<br>
path<br>
pd.read_csv(path)<br>
teachers = pd.read_csv(path)<br>
teachers.columns<br>
teachers.index<br>
teachers = pd.read_csv(path, index_col=0)<br>
teachers<br>
teachers.index<br>
%clear<br>
teachers<br>
teachers[:,2]<br>
teachers<br>
np.arange(12)<br>
import numpy as np<br>
np.arange(12)<br>
np.arange(12).reshape(3,4)<br>
mat = np.arange(12).reshape(3,4)<br>
mat[0, 2]<br>
mat[0,:]<br>
mat[:,1]<br>
mat[1, [0, 2, 3]]<br>
teachers<br>
teachers[[1,2]:]<br>
%clear<br>
teachers<br>
teachers[1:,:]<br>
%clear<br>
teachers<br>
teachers[1:]<br>
teachers[1:3]<br>
teachers[1:2]
teachers
teachers[1:3]
teachers[1:]
teachers['BI':'DB']
teachers
teachers['name']
type(teachers['name'])
teachers['age']
teachers['major']
teachers[['major', 'age']]
teachers
selectedColumns = [['name', 'family', 'age']]
teachers[selectedColumns]
selectedColumns = ['name', 'family', 'age']
teachers[selectedColumns]
teachers.age
teachers.name
teachers.major
teachers
%clear
teachers
teachers[1:3]
teachers[1:3][['name', 'family']]
teachers[['name', 'family']]
df = teachers[['name', 'family']]
df
df[1:3]
teachers[['name', 'family']][1:3]
%clear
# teachers.loc
# teachers.iloc
teachers
teachers.loc['DB']
teachers.loc['name']
teachers.loc[:, 'name']
teachers.loc['DS']
teachers.loc[['DS']]
teachers.loc['BI':'DB']
teachers.loc['BI':'DB', :]
teachers.loc[:, 'name':'age']
teachers.loc[:, ['name','age']]
teachers
teachers.iloc[1:2, :]
teachers.iloc[1:3, :]
teachers.iloc[1:3, 2:4]
teachers.iloc[1:3, [2,4]]
teachers.iloc[1:3, [2,3]]
pd.read_csv(r'H:\Work\Python\Examples\1-basics\cars.csv') # raw text
pd.read_csv(r'H:\Work\Python\Examples\1-basics\cars.csv', index_col = 0) # raw text
cars = pd.read_csv(r'H:\Work\Python\Examples\1-basics\cars.csv', index_col = 0) # raw text
%clear
cars.country
cars['country']
cars[['country']]
cars
cars.iloc[:, 1]
cars
cars.loc[:, 'country']
cars.loc[:, 'country':'drives Right']
cars.loc[:, 'country':'drives right']
cars.iloc[:, 1:]
cars
cars[5:6]
cars[5:6]['drives right']
np.arange(5)
nums = np.arange(5)
nums
nums[3]
nums[-2]
nums[-1]
cars
cars[-2:-1]
cars[-2:-1]['drives right']
cars
%clear
# >, <, ==, >=, <=, !=
'ali' == 'Ali'
3 < 12
5 > 12
# and, or, not
5 == 12
not 5 == 12
5 != 12
5 > 3 and 5 < 7
2 > 7
2 > 7 | 4 < 5
2 > 7 or 4 < 5
nums
nums = np.arange(10)
nums
numsu > 5
nums > 5
nums[nums > 5]
nums
nums > 2 and nums < 7
# np.logical_and()
# np.logical_or()
# np.logical_not()
np.logical_and(nums > 2, nums < 7)
nums[np.logical_and(nums > 2, nums < 7)]
nums
%clear
cars
cars['cars per cap']
cars['cars per cap'] > 500
cars[cars['cars per cap'] > 500]
cars
cars['cars per cap']
np.logical_and(cars['cars per cap'] > 100, cars['cars per cap'] < 500)
cars[np.logical_and(cars['cars per cap'] > 100, cars['cars per cap'] < 500)]
%clear
x = 6
if x < 2:
    True
x = 6
if x < 2:
    True
else:
    False
x = 6
if x < 2:
    flag = True
else:
    flag = False

flag
x = 0
if x < 2:
    flag = True
else:
    flag = False

flag
x = 1
if x % 2 == 0:
    print('dividable by 2')
else:
    print('not dividable by 2')
x = 2
if x % 2 == 0:
    print('dividable by 2')
else:
    print('not dividable by 2')
x = 1
if x % 2 == 0:
    print('dividable by 2')
elif x % 3 == 0:
    print('dividable by 3')
else:
    print('neither dividable by 2 nor 3')
x = 2
if x % 2 == 0:
    print('dividable by 2')
elif x % 3 == 0:
    print('dividable by 3')
else:
    print('neither dividable by 2 nor 3')
x = 3
if x % 2 == 0:
    print('dividable by 2')
elif x % 3 == 0:
    print('dividable by 3')
else:
    print('neither dividable by 2 nor 3')
x = 4
if x % 2 == 0:
    print('dividable by 2')
elif x % 3 == 0:
    print('dividable by 3')
else:
    print('neither dividable by 2 nor 3')
x = 5
if x % 2 == 0:
    print('dividable by 2')
elif x % 3 == 0:
    print('dividable by 3')
else:
    print('neither dividable by 2 nor 3')
x = 1
while x < 10:
    print(x)
x = 1
while x < 10:
    print(x)
    x += 1 # x = x + 1
print(x)
error = 50

while error > 1:
    print(error)
    error /= 4 # error = error / 4

print(error)<br>
names = ['Ali', 'Babak', 'Fatemeh', 'Mosa', 'Maryam', 'Taha', 'Tahere']<br>
names = ['Ali', 'Babak', 'Fatemeh', 'Mosa', 'Maryam', 'Taha', 'Tahere']<br>
for valu in names:<br>
    print(name)<br>
names = ['Ali', 'Babak', 'Fatemeh', 'Mosa', 'Maryam', 'Taha', 'Tahere']<br>
for value in names:<br>
    print(value)<br>
for x in names:<br>
    print(x)
for alaki in names:
    print(alaki)
for name in names:
    print(name)
for name in names:
    print(name)
    if name == "taha":
        print("found!")
        break
for name in names:<br>
    print(name)<br>
    if name == "Taha":<br>
        print("found!")<br>
        break<br>
for name in names:<br>
    if name == "Taha":<br>
        continue<br>
    print(name)<br>
ind = 0<br>
for name in names:<br>
    print(ind, name, sep = ": ")<br>
    ind += 1<br>
len(names)<br>
for num in len(names):<br>
    print(num)
range(len(names))
for num in range(len(names)):
    print(num)
for ind in range(len(names)):
    print(ind, names[ind], sep = ": ")
for value in enumerate(names):<br>
    print(value)<br>
nums = [1, 2]<br>
nums<br>
num1, num2 = nums<br>
num1<br>
num2<br>
for index, name in enumerate(names):<br>
    print(index, name, sep = ": ")<br>
nums = [1, 2, 3, 4]<br>
a, b, c,  d = nums<br>
a<br>
b<br>
c<br>
d<br>
enumerate(names)<br>
type(enumerate(names))<br>
range(10)<br>
list(range(10))<br>
list(enumerate(names))<br>
len(list(enumerate(names)))<br>
house = [["hallway", 11.25], <br>
         ["kitchen", 18.0], <br>
         ["living room", 20.0], <br>
         ["bedroom", 10.75], <br>
         ["bathroom", 9.50]]<br>
for value in house:<br>
    print(value)<br>
for room, size in house:<br>
    print(room, size, sep = ": ")<br>
%clear<br>
matrix = np.arange(9).reshape(3, 3)<br>
matrix<br>
for value in enumerate(matrix):<br>
    print(value)<br>
for rowIndex, row in enumerate(matrix):<br>
    for value in enumerate(row):<br>
        print(value)<br>
matrix<br>
for rowIndex, row in enumerate(matrix):<br>
    for colIndex, value in enumerate(row):<br>
        print("(", str(rowIndex), ', ', str(colIndex), '): ', str(value))<br>
for rowIndex, row in enumerate(matrix):<br>
    for colIndex, value in enumerate(row):<br>
        print("(", str(rowIndex), ', ', str(colIndex), '): ', str(value), sep = "")<br>
for char in "Seyyedeh Maryam Hosseini":
    print(char)
house
houseDict = {}
for room, size in house:
    houseDict[room] = size
houseDict
for value in houseDict:
    print(value)
for key in houseDict:
    print(houseDict[key])
for key in houseDict:
    print(key, houseDict[key], sep = ": ")
for key in houseDict.keys():
    print(key)
for value in houseDict.values():
    print(value)
for value in houseDict.itmes():
    print(value)
for value in houseDict.items():
    print(value)
for key, value in houseDict.items():
    print(key, value, sep = ": ")
%clear
dict(house)
%clear
nums = [223, 108, 95]
np.array(nums)
npNums = np.array(nums)
for num in npNums:
    print(num)
height = [1.84, 1.78, 2.05]
weight = [76, 83, 105]
height = [1.84, 1.78, 2.05]
weight = [76, 83, 105]
npInfo = np.array([height, weight])
for value in npInfo:
    print(value)
for value in npInfo.T:
    print(value)
for value in npInfo:
    print(value)
for row in npInfo:
    for value in row:
        print(value)
npInfo.reshape(-1)
for value in npInfo.reshape(-1):
    print(value)
for value in np.nditer(npInfo):
    print(value)
teachers
for value in teachers:
    print(value)
for column in teachers:
    print(teachers[column])
    print("==============")
for column in teachers:
    print(teachers[row:])
    print("==============")
for row in teachers:
    print(teachers[row:])
    print("==============")
teachers.index
teachers.shape
teachers.shape[0]
for rowIndex in range(teachers.shape[0]):
    print(teachers.iloc[rowIndex,:])
    print("==============")
teachers.index
for rowIndex in teachers.index:
    print(rowIndex)
for rowIndex in teachers.index:
    print(teachers.loc[rowIndex, :])
for rowIndex in teachers.index:
    print(teachers.loc[rowIndex, :])
    print("==============")
teachers.iterrows()
for value in teachers.iterrows():
    print(value)
for value in teachers.iterrows():
    print(value)
    print("==============")
for rowIndex, row in teachers.iterrows():
    print(row)
    print("==============")
for rowIndex, row in teachers.iterrows():
    print(rowIndex)
    print("==============")
%clear
teachers
# DS: Ali Sadeghi Aghili
# BI: Babak Pirooz
for col in teachers.index:    
    print(col,teachers.loc[col,"name":"family"], sep=": ")
for rowIndex, row in teachers.iterrows():    
    print(rowIndex, row,[:2], sep = ":")
for rowIndex, row in teachers.iterrows():    
    print(rowIndex, row[,:2], sep = ":")
for rowindex, row in techers.itrrows(): 
    print(rowindex, row, sep=" :")
for rowindex, row in techers.itrrows(): 
    print(row['name'], row['family'])
for rowindex, row in teachers.itrrows(): 
    print(row['name'], row['family'])
for rowindex, row in teachers.iterrows(): 
    print(row['name'], row['family'])
for rowindex, row in teachers.iterrows(): 
    print(rowIndex, row['name'], row['family'])
for rowindex, row in teachers.iterrows(): 
    print(rowindex, row['name'], row['family'])
for rowindex, row in teachers.iterrows(): 
    print(rowindex + ': ' + row['name'] + ' ' + row['family'])
teachers
teachers['user'] = "user001"
teachers
del teachers['user']
teachers
for rowIndex, row in teachers.iterrows():    
    row['count'] = len(row['name'])
teachers
for rowIndex, row in teachers.iterrows():    
    row['count'] = len(row['name'])
teachers
teachers['count'] = 0
for rowIndex, row in teachers.iterrows():    
    row['count'] = len(row['name'])
teachers<br>
name_lengths = []<br>
for name in teachers['name']:<br>    
    name_lengths.append(len(name))<br>
name_lengths<br>
teachers['count'] = name_lengths<br>
teachers<br>
for rowIndex, row in teachers.iterrows():    <br>
    teachers.loc[rowIndex, 'count2'] = len(row['name'])<br>
teachers<br>
%clear<br>
for rowIndex, row in teachers.iterrows():    
    # teachers.loc[rowIndex, 'count2'] = len(row['name'])    
    row['count2'] = len(row['name'])
teachers
for rowIndex, row in teachers.iterrows():    
    # teachers.loc[rowIndex, 'count2'] = len(row['name'])    
    row['count3'] = len(row['name'])
teachers
teachers.name<br>
teachers.name.apply(len)<br>
teachers['count3'] = teachers.name.apply(len)<br>
teachers<br>
len(teachers.name)<br>
len("ali sadeghi")<br>
cars<br>
cars.country<br>
cars.country.apply(upper)<br>
"Ali Sadeghi Aghili".upper()<br>
cars.country.apply(str.upper)<br>
for rowIndex, row in cars.iterrows():<br>
    cars.loc[rowIndex,'capital'] = row['country'].upper()<br>
cars<br>














