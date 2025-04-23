## Data Processing with Python <br>

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

Funtions:(indentation is very important)<br>
def FuncName(arg):<br>
    return(expr)<br>

Sometimes arg is not needed, <br>
e.g: # Current date and time<br>
now = datetime.now()<br>

explanation about Functions:<br>
help(sum)<br>
?sum<br>
SPYDER---> tools-->preferences--->Help--> active all sections<br>

a---> z : z has bigger Ascii code for sorting (Ascci code of Capital letter is bigger than small letter A > a)<br>
len(lst) number of elements in mentioned list <br>
sorted(lst, reverse=True)<br>
<br>
using cheat sheet is very important<br>
<br>
String Methods:<br>
'ali'.capitilize<br>
'ali'.upper()<br>
'Ali'.lower()<br>
'maryam hosseini'.count('a')<br>
'maryam hosseini'.count('gh')<br>
'maryam hosseini'.index('i')<br>
'maryam hosseini'.index('i',3) ---> from third element afterward<br>
'maryam hosseini'.split() ---> split by distance<br>
'maryam hosseini'.split('i') ---> split by i<br>
list('maryam hosseini') break down into each letter<br>

Iterable / Iterator<br>
# gready methods<br>
lst = [1,2,1,3,1,4]<br>
lst.index<br>
lst.count(1)<br>
lst.append(1)<br>
lst.remove(1)<br>
lst.reverse()<br>


lst.pop()<br>
lst.pop(index)<br>

# Dictionary : pair of key, value (key,value)<br>
DictName.keys()---> key<br>
DictName.values()---> value<br>
DictName.items() ---> (key,value)<br>

DictName[key] ---> value<br>
for slicing a dictionary by Index, it should be converted to a list<br>
a dictinary works by keys and a list works by indexes<br>

list(DictName.keys())[0]<br>
list(DictName.items())[0][0]<br>

# adding new item to a dict<br>
DictName[key]=value <br>
# deleting an item from a dict<br>
del DictName[key]<br>
DictName[key].pop(key)<br>
# changing an item in a dict<br>
DictName[key]= new value <br>

*When order is important ,we use **lists** and when finding values based on keys is important, **Dictionaries** should be considered.*<br>
*NOSQL logic is using several nested Dictionaries*<br>

Example of a nested dictionary:<br>
italy = {'capital': 'rome', 'population': 59.83 }<br>
spain = {'capital': 'madrid', 'population': 46.77 }<br>
france = {'capital': 'paris', 'population': 66.03 }<br>
germany= {'capital': 'berlin', 'population': 80.62 }<br>
norway= {'capital': 'oslo', 'population': 5.084 }<br>
europe = {'italy': italy, 'spain': spain, 'france': france, 'germany': germany, 'norway': norway}<br>
europe<br>
europe['france']<br>
result = europe['france']<br>
result<br>
result['capital']<br>
europe['france']<br>
europe['france']['capital']<br>

# "in" applications<br>
'Ali' in 'alireza'   ---> False<br>
'Ali'.lower() in 'alireza' ---> True<br>
lst = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10<br>
5 in lst   ---> True<br>
11 in lst  ---> False<br>
lst2 = ['ali', 'sadeghi']<br>
'ali' in lst2  ---> True<br>
'akbar' in lst2  ---> False<br>
familyDict<br>
familyDict['father'] = 175<br>
familyDict<br>
175 in familyDict  ---> True<br>
'father' in familyDict  ---> False<br>
'son2' in familyDict  ---> True<br>
'180' in familyDict  ---> False<br>
familyDict.values()  <br>
170 in familyDict.values()  ---> True<br>

import numpy<br>
heights = [184, 175]<br>
weights = [76, 66]<br>
BMI = weight/height ** 2<br>
BMI = weights/heights ** 2<br>
weights[0]/heights[0] ** <br>
weights[1]/heights[1] ** 2<br>
weights[0]/(heights[0]/100) ** 2<br>
weights[1]/(heights[1]/100) ** 2<br>
BMI = [bmi1, bmi2]<br>
bmi1 = weights[0]/(heights[0]/100) ** 2<br>
bmi2 = weights[1]/(heights[1]/100) ** 2<br>
BMI = [bmi1, bmi2]<br>
BMI<br>
def multiply(lst1, lst2):<br>
    y = <br>
    lst = <br>
        for element1 in lst1:<br>
            for element2 in lst2:<br>
                multiply = element1 * element2<br>
                lst.append(multiply)<br>
                y += 1<br>
                break<br>
    return lst<br>
def multiply(lst1, lst2):<br>
    y = 0<br>
    lst = []<br>
    for element1 in lst1:<br>
        for element2 in lst2:<br>
            multiply = element1 * element2<br>
            lst.append(multiply)<br>
            y += 1<br>
            break<br>
    return lst<br>
multiply(num1, num2)<br>
num1 = [1, 2, 3]<br>
num2 = [1, 2, 3]<br>
multiply(num1, num2)<br>
def multiply(lst1, lst2):<br>
    y = 0<br>
    lst = []<br>
    for element1 in lst1:<br>
        for element2 in lst2[y:]:<br>
            multiply = element1 * element2<br>
            lst.append(multiply)<br>
            y += 1<br>
            break<br>
    return lst<br>
multiply(num1, num2)<br>
npNum1 = np.array(num1)<br>
import numpy as np<br>
npNum1 = np.array(<br>
npNum1 = np.array(num1)<br>
npNum2 = np.array(num2)<br>
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
v1 = np.random.rand(100000)<br>
v2 = np.random.rand(100000)<br>
%time multiply(v1,v2)<br>
%time a = multiply(v1,v2)<br>
v1 = np.random.rand(1000000)<br>
v2 = np.random.rand(1000000)<br>
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
range(10)<br>
type(range(10))<br>
list(range(10))<br>
list(range(10, 20))<br>
list(range(10, 20, 2))<br>
np.arange(10)<br>
np.arange(10, 20)<br>
np.arange(10, 20, 2)<br>
np.arange(12)<br>
lst = [[0, 1, 2, 3, 4, 5], [6, 7, 8, 9, 10, 11]]<br>
np.array(lst)<br>
np.arange(12)<br>
np.arange(12).reshape(2, 6)<br>
np2d = np.arange(12).reshape(2, 6)<br>
np2d<br>
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

## ---(Fri Nov  1 13:57:51 2024)---
%clear
1, 2, 3
type((1, 2, 3))
(1, 'ali', 3.14, True)
a, b, c = (1, 2, 3)
a
b
c
def powerBoth(num1, num2):
    tup = (num1 ** num2, num2 ** num1)
    return tup
powerBoth(2, 3)
powerBoth(2, 3)[0]
powerBoth(2, 3)[1]
%clear
tweets = pd.read_csv(r'H:\Work\Python\Examples\1-basics\tweets.csv')
import pandas as pd
tweets = pd.read_csv(r'H:\Work\Python\Examples\1-basics\tweets.csv')
tweets
tweets.lang
langDict = {}
for lang in tweets.lang:
    print(lang)
langDict = {}
for lang in tweets.lang:
    if lang not in langDict:
        langDict[lang] = 1
    else:
        langDict[lang] += 1
langDict
%clear
newValue = 10

def square(val):
    newValue = value ** 2
    return newValue
newValue
square(3)
def square(value):
    newValue = value ** 2
    return newValue
square(3)
def mod2(num1, num2, num3):
    mod1 = num1 % 2
    mod2 = num2 % 2
    mod3 = num3 % 2
    
    return(mod1, mod2, mod3)
mod(10, 11, 12)
mod2(10, 11, 12)
def mod(num):
    return num % 2

def mod2(num1, num2, num3):
    return(mod(num1), mod(num2), mod(num3))
mod2(10, 11, 12)
def mod2(num1, num2, num3):
    def inner(num):
        return num % 2
    
    return(inner(num1), inner(num2), inner(num3))
mod2(10, 11, 12)
def xpowy(y):
    def inner(x):
        return x ** y
    return inner
xpowy(2)
square = xpowy(2)
square(12)
square(5)
square(6)
cubic = xpowy(3)
cubic(5)
cubic(3)
cubic(2)
def factorial(num):
    if num in [0, 1]:
        return 1
    else:
        return num * factorial(num - 1)
factorial(0)
factorial(1)
factorial(13)
factorial(3)
factorial(5)
5 * 4 * 3 * 2
sum([1, 2, 3, 4 , 5])
def summation(num1, num2, num3):
    total = 0
    for num in [num1, num2, num3]:
        total += num
    return total
summation(1, 2, 3)
summation(1, 2, 3, 4)
def summation(*nums):
    print(nums)
summation(10, 11, 12, 13, 14)
def summation(*nums):
    total = 0
    for num in nums:
        total += num
    return total
summation(1)
summation(1, 2)
summation(1, 2, 3)
summation(1, 2, 3, 4)
summation(1, 2, 3, 4, 5)
summation(1, 2, 3, 4, 5, 6)
def alaki(**entery):
    return entery
alaki(name = "ali", age = 36, family = "sadeghi")
%clear
def multiply(*nums):
    if 0 in nums:
        return 0
    else:
        total = 1
        for num in nums:
            total *= num
    
    return num
echo('ali', 4)
def echo (word, rep):
    return word * rep
echo('ali', 4)
echo2 = lambda word, rep: word * rep
echo2('ali', 4)
nums = (1, 2, 3, 4)
nums
map(lambda num: num ** 2, nums)
result = map(lambda num: num ** 2, nums)
result
type(result)
list(result)
def square(num):
    return num ** 2
list(map(square, nums))
nums = range(-5, 5)
filter(lambda num: num < 0, nums)
result = filter(lambda num: num < 0, nums)
type(result)
list(result)
result = filter(lambda num: num % 2 == 0, nums)
list(result)
%clear
map(lambda num1, num2: num1 + num2, nums1, nums2)
nums1 = [4, 5, 6]
nums1 = [6, 5, 4]
# result = [10, 10, 10]

map(lambda num1, num2: num1 + num2, nums1, nums2)
nums1 = [4, 5, 6]
nums2 = [6, 5, 4]
# result = [10, 10, 10]

map(lambda num1, num2: num1 + num2, nums1, nums2)

"""
Created on Fri Nov  1 15:49:09 2024

@author: ali sadeghi aghili
"""
nums1 = [4, 5, 6]
nums2 = [6, 5, 4]
# result = [10, 10, 10]

list(map(lambda num1, num2: num1 + num2, nums1, nums2))
teachers
teacher
pd.read_csv(r'H:\Work\Python\Examples\1-basics\teachers.csv').name
names = pd.read_csv(r'H:\Work\Python\Examples\1-basics\teachers.csv').name
list(map(lambda name: len(name) > 4, names))
list(filter(lambda name: len(name) > 4, names))
gap = pd.read_csv(r'H:\Work\Python\Examples\1-basics\gapminder.csv')
gap
gap.country.map(len)
gap.country.apply(len)
gap.columns
gap.loc[:, ['life_exp', 'gdp_cap']].apply(lambda num: num + 10, axis = 0)
gap.loc[:, ['life_exp', 'gdp_cap']]
gap.applymap(lambda num: num + 10)
gap.applymap(lambda num: str(num) + 10)
gap.applymap(lambda num: str(num) + '10')
nums = [43, 11, 49, 13]
reduce(lambda num1, num2: num1 if num1 > num2 else num2, nums)
from functools import reduce
nums = [43, 11, 49, 13]
reduce(lambda num1, num2: num1 if num1 > num2 else num2, nums)
reduce(lambda num1, num2: num1 * num2, nums)
names = ['Ali', 'Babak', 'Fatehemh', 'Mosa', 'Maryam', 'Taha', 'Tahere']
for name in names:
    print(name)
namesIter = iter(names)
namesIter
next(namesIter)
namesIter = iter(names)
next(namesIter)
print(* namesIter)
nums1 = [4, 5, 6]
nums2 = [6, 5, 4]
result = map(lambda num1, num2: num1 + num2, nums1, nums2)
next(result)
%clear
names = ['Ali', 'Babak', 'Fatehemh', 'Mosa', 'Maryam', 'Taha', 'Tahere']
family = ['Ghasemi', 'Javanmard', 'Khani', 'Naseri']
age = [40, 34]
zip(names, family, age)
list(zip(names, family, age))
names = ['Ali', 'Babak', 'Fatehemh', 'Mosa', 'Maryam', 'Taha', 'Tahere']
family = ['Ghasemi', 'Javanmard', 'Khani', 'Naseri']
age = [40, 34, 0, 0, 0]
list(zip(names, family, age))
for info in zip(names, family, age):
    print(info)
for name, family, age in zip(names, family, age):
    print(name + ' ' + family + ': ' + str(age))
provinces
provinces = ['Eastern Azarbaijan', 'Western Azarbaijan', 'Ardabil', 'Isfahan',
             'Alborz', 'Ilam', 'Bushehr', 'Tehran', 'Charmahal & Bakhtiari',
             'Southern Khorasan', 'Razavian Khorasan', 'Northern Khorasan',
             'Khuzestan', 'Zanjan', 'Semnan', 'Sistan & Balouchestan', 'Fars',
             'Qazvin', 'Qom', 'Kurdistan', 'Kerman', 'Kermanshah',
             'Kohgiluye & Boyer Ahmad', 'Golestan', 'Gilan', 'Lorestan',
             'Mazandaran', 'Markazi', 'Hormozgan', 'Hamedan', 'Yazd']

cities = ['Tabriz', 'Oroumieh', 'Ardabil', 'Isfahan', 'Karaj', 'Ilam', 'Bushehr',
          'Tehran', 'Shahre Kord', 'Birjand', 'Mashad', 'Bojnourd', 'Ahwaz',
          'Zanjan', 'Semnan', 'Zahedan', 'Shiraz', 'Qazvin', 'Qom', 'Sanandaj',
          'Kerman', 'Kermanshah', 'Yasouj', 'Gorgan', 'Rasht', 'Khorram Abad',
          'Saari', 'Arak', 'Bandar Abbas', 'Hamedan', 'Yazd']
dict(zip(provinces, cities))
info = zip(provinces, cities)
next(info)
province , city = next(info)
province
city
province , city = next(info)
province
city
pd.read_csv(r'H:\Work\Python\Examples\1-basics\tweets.alaki')
pd.read_csv(r'H:\Work\Python\Examples\1-basics\tweets')
for chunk in pd.read_csv(r'H:\Work\Python\Examples\1-basics\tweets.csv', chunksize=10):
    print(chunk)
    print('=====================================')
for chunk in pd.read_csv(r'H:\Work\Python\Examples\1-basics\data.csv', chunksize=500):
    print(chunk.iloc[:, 0])
    print('=====================================')
total = 0
for chunk in pd.read_csv(r'H:\Work\Python\Examples\1-basics\data.csv', chunksize=500):
    total += sum(chunk.iloc[:, 0])
    print(total)
    print('=====================================')
result = []
for value in [1, 2, 3, 4]:
    result.append(value * 10)
result
[]
type([])
[value * 10 for value in [1, 2, 3, 4]]
result = [value * 10 for value in [1, 2, 3, 4]]
result
pairs = []
for num1 in range(0, 2):
    for num2 in range(6, 8):
        pairs.append(num1, num2)
pairs = []
for num1 in range(0, 2):
    for num2 in range(6, 8):
        pairs.append((num1, num2))
pairs
[(num1, num2) for num1 in range(0, 2) for num2 in range(6, 8)]
[num ** 2 for num in range(5)]
[num ** 2 for num in range(10)]
len([num ** 2 for num in range(10)])
[num ** 2 for num in range(10)]
[num ** 2 for num in range(10) if num % 2 == 0]
len([num ** 2 for num in range(10) if num % 2 == 0])
[num ** 2 if num % 2 == 0 else num for num in range(10)]
[[[num],[num],[num],[num]] for num in range(4)]
[[num],[num],[num],[num] for num in range(4)]
[[num,num,num,num] for num in range(4)]
[num for num in range(4)]
[[] for num in range(4)]
[[num2 for num2 in range(4)] for num1 in range(4)]
[[row + col for col in range(4)] for row in range(4)]
[[row * 4 + col for col in range(4)] for row in range(4)]
teachers
pd.read_csv(r'H:\Work\Python\Examples\1-basics\teachers.csv')
teachers = pd.read_csv(r'H:\Work\Python\Examples\1-basics\teachers.csv', index_col = 0)
teachers
[name for name in teachers.name]
[name for name in teachers.name if len(name) > 4]
{num:-num for num in range(4)}
{num:[] for num in range(4)}
teachers
{name + ' ' + family: major for name, family, major in zip(teachers.name, teachers.family, teachers.major)}
[(name, family, major) for name, family, major in teachers]
teachers
numGen = (num for num in range(6))
next(numGen)
[num for num in range(10 ** 100)]<br>
[num for num in range(10 ** 10)]<br>
numGen = (num for num in range(10 ** 100000))<br>
next(numGen)<br>
def numSeq(num):<br>
    ind = 0<br>
    while ind < num:<br>
        yield ind<br>
        ind += 1<br>
numSeq(5)<br>
result = numSeq(5)<br>
next(result)<br>
teachers<br>
def nameCount (names):  <br>  
    for name in names:<br>
        yield len(name)<br>
result = nameCound(teachers.name)<br>
result = nameCount(teachers.name)<br>
next(result)<br>
nameLenGen =(len(name) for name in teachers.name)<br>
next(nameLenGen)<br>












