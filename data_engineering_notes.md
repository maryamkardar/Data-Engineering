## Data Processing with Python <br>

First Session:🙌<br>

print("your BMI is:",{BMI})<br>
print(f"your BMI is: {BMI}")<br>
print('your BMI is:' + str(BMI))<br>
print("your BMI is", BMI, sep= ":")<br>

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
npNum1 * npNum2<br>
np.random.rand(10)<br>
v1 = np.random.rand(1000000)<br>
v2 = np.random.rand(1000000)<br>
v1 = np.random.rand(100000)<br>
v2 = np.random.rand(100000)<br>
# Magic commands on IPYTHON<br>
%time v1 * v2<br>
v1 = np.random.rand(1000000)<br>
v2 = np.random.rand(1000000)<br>
%time v1 * v2<br>
v1 = np.random.rand(100000)<br>
v2 = np.random.rand(100000)<br>
%time multiply(v1,v2)<br>
%time a = multiply(v1,v2)<br>
v1 = np.random.rand(1000000)<br>
v2 = np.random.rand(1000000)<br>
%time v1 * v2<br>
npHeights = np.array(heights)<br>
npWeights = np.array(weights)<br>
BMI = npWeights/npHeights ** 2<br>
BMI<br>
BMI = npWeights/(npHeights/100) ** 2<br>
BMI<br>
BMI[0]<br>
BMI[1]<br>
npHeights[0]<br>
type(npHeights)<br>
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
np2d.reshape(-1,)  *reshape 2 dimension into one dimension*<br>
np2d.reshape(3, 4)<br>
np2d = np2d.reshape(3, 4)<br>
np2d<br>
# Slicing in NUMPY<br>
np2d[1]<br>
np2d[1][2]<br>
np2d[1, 2]<br>
np2d<br>
np2d[2]<br>
np2d[2][:]<br>
np2d[2, :]<br>
np2d<br>
np2d[:,2]<br>
%clear<br>
np2d<br>
np2d.transpose()<br>
np2d.T<br>
%clear<br>
weight<br>
height<br>
npWeight = np.array(weight)<br>
npHeight = np.array(height)<br>
BMI = npWeight / npHeight ** 2<br>
BMI<br>
BMI = npWeight * 0.453592 / (npHeight * 0.0254) ** 2<br>
BMI<br>
np.array([weight, height])<br>
np.array([weight, height]).T<br>
np.array([weight, height]).T * np.array([0.453592, 0.0254])<br>
info = np.array([weight, height]).T * np.array([0.453592, 0.0254])<br>
info [:, 1] / info[:, 2] ** 2<br>
info [:, 0] / info[:, 1] ** 2<br>
2 > 3<br>
2 < 5<br>
[1, 2, 3, 4, 5, 6]<br>
[1, 2, 3, 4, 5, 6] > 3<br>
# recycling<br>
# broadcasting<br>
np.array([1, 2, 3, 4, 5, 6])<br>
np.array([1, 2, 3, 4, 5, 6]) > 3<br>
np.array([1, 2, 3, 4, 5, 6]) > np.array([3, 3, 3, 3, 3, 3])<br>
BMI<br>
BMI < 22<br>
len(BMI)<br>
BMI[BMI < 22]<br>
np.array([1, 2, 3, 4, 5, 6]) > 3<br>
lst = np.array([1, 2, 3, 4, 5, 6])<br>
lst > 3<br>
lst[lst > 3]<br>
info<br>
info.ndim<br>
info.shape<br>
info.size<br>
len(info)<br>
np.array([weight, height])<br>
npWeight<br>
npHeight<br>
np.column_stack((npWeight, npHeight))
np.row_stack((npWeight, npHeight))
nums = np.arange(200)
nums
np.mean(nums)<br>
nums.mean()<br>
np.std(nums)<br>
nums.std()<br>
np.abs([-12, 2, 5, -3])<br>
[-12, 2, 5, -3].abs()<br>
np.array([-12, 2, 5, -3]).abs()<br>
np.max(nums)<br>
nums.max()<br>
np.median(nums)<br>
nums.median()<br>
%clear<br>
height<br>
weight<br>
age<br>
position<br>
num1<br>
lst1<br>
v1<br>
v2<br>
v1 * v2<br>
np.dot(v1, v2)<br>
a1 = np.array([1, 2, 3, 4]).reshape(2, 2)<br>
a1<br>
a2 = np.array([1, 2, 3, 4]).reshape(2, 2)<br>
np.cross(a1, a2)<br>
np.matrix()<br>
np.matrix(range(100))<br>
np.matrix(range(100)).reshape(4, 25)<br>

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
teachers<br>
teachers['name']<br>
type(teachers['name'])<br>
teachers['age']<br>
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

flag<br>
x = 0<br>
if x < 2:<br>
    flag = True<br>
else:<br>
    flag = False<br>

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
for rowIndex, row in teachers.iterrows():<br>
    print(rowIndex)<br>
    print("==============")<br>
%clear<br>
teachers<br>
# DS: Ali Sadeghi Aghili<br>
# BI: Babak Pirooz<br>
for col in teachers.index:<br>    
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
    return tup<br>
powerBoth(2, 3)<br>
powerBoth(2, 3)[0]<br>
powerBoth(2, 3)[1]<br>
%clear<br>
tweets = pd.read_csv(r'H:\Work\Python\Examples\1-basics\tweets.csv')<br>
import pandas as pd<br>
tweets = pd.read_csv(r'H:\Work\Python\Examples\1-basics\tweets.csv')<br>
tweets<br>
tweets.lang<br>
langDict = {}<br>
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
    
    return(mod1, mod2, mod3)<br>
mod(10, 11, 12)<br>
mod2(10, 11, 12)<br>
def mod(num):<br>
    return num % 2<br>

def mod2(num1, num2, num3):<br>
    return(mod(num1), mod(num2), mod(num3))<br>
mod2(10, 11, 12)<br>
def mod2(num1, num2, num3):<br>
    def inner(num):<br>
        return num % 2<br>
    
    return(inner(num1), inner(num2), inner(num3))<br>
mod2(10, 11, 12)<br>
def xpowy(y):<br>
    def inner(x):<br>
        return x ** y<br>
    return inner<br>
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



## ---(Thu Nov  7 14:01:41 2024)---<br>
fileHandler = open(r'H:\Work\Python\Examples\2-Importing\Story.txt', 'rt')<br>
fileHandler<br>
fileHandler.read()<br>
fileHandler = open(r'H:\Work\Python\Examples\2-Importing\Story.txt', 'rt')<br>
fileHandler.read()<br>
fileHandler.seek(0)<br>
fileHandler.read()<br>
fileHandler.seek(0)<br>
fileHandler.read()<br>
fileHandler.seek(10)<br>
fileHandler.read()<br>
fileHandler.seek(0)<br>
fileHandler.read(10)<br>
fileHandler.seek(0)<br>
fileHandler.readlines()<br>
fileHandler.seek(0)<br>
lines = fileHandler.readlines()<br>
type(lines)<br>
lines<br>
lines[0]<br>
lines[1]<br>
fileHandler.seek(0)<br>
fileHandler.readline()<br>
fileHandler.read()<br>
fileHandler.seek(0)<br>
fileHandler.readlines()<br>
fileHandler.seek(0)<br>
fileHandler.readline()<br>
# lock<br>
fileHandler.close()<br>
fileHandler = open(r'H:\Work\Python\Examples\2-Importing\Story.txt', 'rt')<br>
fileHandler.readlines(100)<br>
fileHandler.readline()<br>
fileHandler.close()<br>
fileHandler = open(r'H:\Work\Python\Examples\2-Importing\Story.txt', 'rt')<br>
lines = fileHandler.readlines()<br>
lines<br>
line[0]<br>
lines[0]<br>
lines[0:5]<br>
fileWriter = open(r'H:\Work\Python\Examples\2-Importing\empty.txt', 'wt')<br>
fileWriter.write('hi.')<br>
fileWriter.close()<br>
fileWriter = open(r'H:\Work\Python\Examples\2-Importing\empty.txt', 'wt')<br>
fileWriter.write('Hello to you!')<br>
fileWriter.close()<br>
fileWriter = open(r'H:\Work\Python\Examples\2-Importing\empty.txt', 'wt')<br>
fileWriter.write('Hello to you!')<br>
fileWriter.write('\n')<br>
fileWriter.write('How is everything?\n')<br>
fileWriter.close()<br>
fileWriter = open(r'H:\Work\Python\Examples\2-Importing\empty.txt', 'wt')<br>
fileWriter.write('Hello to you!')<br>
fileWriter.write('\n')<br>
fileWriter.write('How is everything?\n')<br>
fileWriter.seek(15)<br>
fileWriter.write('This is Ali.\n')<br>
fileWriter.close()<br>
fileWriter = open(r'H:\Work\Python\Examples\2-Importing\empty.txt', 'wt')<br>
fileWriter.write('Hello to you!')<br>
fileWriter.write('\n')<br>
fileWriter.write('How is everything?\n')<br>
fileWriter.seek(15)<br>
fileWriter.write('This is Ali.\n')<br>
fileWriter.write('We are testing some new things.\n')<br>
fileWriter.close()<br>
fileWriter = open(r'H:\Work\Python\Examples\2-Importing\empty.txt', 'wt')<br>
fileWriter.writelines(['Hello to you!', 'How is everything?', 'This is Ali.', 
                       'We are testing some new things.'])
fileWriter.close()<br>
?open.writelines<br>
?fileWriter.writelines<br>
help(fileWriter.writelines)<br>
fileWriter = open(r'H:\Work\Python\Examples\2-Importing\empty.txt', 'wt')<br>
fileWriter.writelines(['Hello to you!', 'How is everything?', 'This is Ali.', 
                       'We are testing some new things.'], '\n')
fileWriter.close()
fileWriter = open(r'H:\Work\Python\Examples\2-Importing\empty.txt', 'wt')<br>
fileWriter.writelines(['Hello to you!\n', 
                       'How is everything?\n', 
                       'This is Ali.\n', 
                       'We are testing some new things.\n'])
fileWriter.close()
fileWriter = open(r'H:\Work\Python\Examples\2-Importing\empty.txt', 'at')
file.write('We are using append method right now.')
fileWriter.write('We are using append method right now.')
fileWriter.close()
fileWriter = open(r'H:\Work\Python\Examples\2-Importing\empty.txt', 'wt')
fileWriter.write('We are using append method right now.')
fileWriter.close()
fileWriter = open(r'H:\Work\Python\Examples\2-Importing\empty.txt', 'wt')
fileWriter.seek(30)
fileWriter.write('We are using append method right now.')
fileWriter.close()
fileWriter = open(r'H:\Work\Python\Examples\2-Importing\empty.txt', 'wt')
fileWriter.write('We are using append method right now.')
fileWriter.close()
fileWriter = open(r'H:\Work\Python\Examples\2-Importing\empty.txt', 'at')
fileWriter.seek(15)
fileWriter.write('||We are using append method right now.')
fileWriter.close()
fileWriter = open(r'H:\Work\Python\Examples\2-Importing\empty.txt', 'rt+')
fileReader = open(r'H:\Work\Python\Examples\2-Importing\empty.txt', 'rt+')
fileReader.read()
fileWriter.write('||We are using append method right now.')
fileReader.close()
fileReader = open(r'H:\Work\Python\Examples\2-Importing\empty.txt', 'rt+')
fileReader.read()
fileReader.write('**akjhdkjhasdkjh**')
fileReader.close()
fileWriter = open(r'H:\Work\Python\Examples\2-Importing\empty.txt', 'wt')
file.read()
fileWriter.read()
fileWriter.write('ali sadeghi')
fileWriter.read()
fileWriter.close()
fileWriter = open(r'H:\Work\Python\Examples\2-Importing\empty.txt', 'wt+')
fileWriter.write('ali sadeghi')
fileWriter.read()
fileWriter.seek(0)
fileWriter.read()
fileWriter.close()
fileWriter = open(r'H:\Work\Python\Examples\2-Importing\empty.txt', 'wt+')
fileWriter.write('ali sadeghi')
fileWriter.seek(0)
fileWriter.read()
fileWriter.write('. this is me.')
fileWriter.close()
# lock
with open(r'H:\Work\Python\Examples\2-Importing\empty.txt', 'wt+') as fileHandler:
    fileHandler.write('ali sadeghi')
    fileHandler.seek(0)
    fileHandler.read()
    fileHandler.write('. this is me.')
    fileHandler.write('. we are testing again.')
np.loadtxt(r'H:\Work\Python\Examples\2-Importing\npTestWithoutHeader.txt')
import numpy as np
np.loadtxt(r'H:\Work\Python\Examples\2-Importing\npTestWithoutHeader.txt')
np.loadtxt(r'H:\Work\Python\Examples\2-Importing\npTestWithoutHeader.txt', delimiter= ',')
np.loadtxt(r'H:\Work\Python\Examples\2-Importing\npTestWithoutHeader.txt', delimiter= ',', dtype = 'int')
np.loadtxt(r'H:\Work\Python\Examples\2-Importing\npTestWithHeader.txt', delimiter= ',', dtype = 'int')
np.loadtxt(r'H:\Work\Python\Examples\2-Importing\npTestWithHeader.txt', 
           delimiter= ',', 
           dtype = 'int',
           skiprows=1)
np.loadtxt(r'H:\Work\Python\Examples\2-Importing\Snapp.txt', 
           delimiter= ',', 
           dtype = 'int')
np.loadtxt(r'H:\Work\Python\Examples\2-Importing\Snapp.txt', 
           delimiter= ',', 
           dtype = 'int',
           skiprows=1)
np.loadtxt(r'H:\Work\Python\Examples\2-Importing\Snapp.txt', 
           delimiter= ',', 
           dtype = 'str',
           skiprows=1)
np.loadtxt(r'H:\Work\Python\Examples\2-Importing\Snapp.txt', 
           delimiter= ',', 
           #dtype = 'str',
           skiprows=1,
           usecols=3)
np.genfromtxt(r'H:\Work\Python\Examples\2-Importing\titanic_sub.csv')
np.genfromtxt(r'H:\Work\Python\Examples\2-Importing\titanic_sub.csv', delimiter=',')
np.genfromtxt(r'H:\Work\Python\Examples\2-Importing\titanic_sub.csv', delimiter=',', skip_header=1)
np.genfromtxt(r'H:\Work\Python\Examples\2-Importing\titanic_sub.csv', delimiter=',', names=True)
np.recfromcsv(r'H:\Work\Python\Examples\2-Importing\titanic_sub.csv')
%clear
np.genfromtxt(r'H:\Work\Python\Examples\2-Importing\titanic_sub.csv', delimiter=',', names=True)
np.recfromcsv(r'H:\Work\Python\Examples\2-Importing\titanic_sub.csv')
%clear
# dumping
infoDict = {'Name': 'Ali', 'Family': 'Sadeghi', 'Age': 36}
infoDict
import pickle
pickleWriter = open(r'H:\Work\Python\Examples\2-Importing\alaki.alisadeghi', 'wb')
pickle.dump(infoDict, pickleWriter)
pickleWriter.close()
del infoDict
infoDict
pickleReader = open(r'H:\Work\Python\Examples\2-Importing\alaki.alisadeghi', 'rb')
pickle.load(pickleReader)
infoDict = pickle.load(pickleReader)
pickleReader = open(r'H:\Work\Python\Examples\2-Importing\alaki.alisadeghi', 'rb')
infoDict = pickle.load(pickleReader)
infoDict
pickleReader.close()
infoDict
pd.read_csv(r'H:\Work\Python\Examples\2-Importing\titanic_sub.csv')
import pandas as pd
pd.read_csv(r'H:\Work\Python\Examples\2-Importing\titanic_sub.csv')
pd.read_csv(r'H:\Work\Python\Examples\2-Importing\titanic_sub.csv', index_col=0)
titanic = pd.read_csv(r'H:\Work\Python\Examples\2-Importing\titanic_sub.csv', index_col=0)
titanic
pd.to_pickle(titanic, pickleWriter)
pickleWriter = open(r'H:\Work\Python\Examples\2-Importing\titanic.pkl', 'wb')
pd.to_pickle(titanic, pickleWriter)
pickleWriter.close()
del titanic
pickleReader = open(r'H:\Work\Python\Examples\2-Importing\titanic.pkl', 'rb')
titanic = pickle.load(pickleReader)
pickleReader.close()
titanic
path = r'H:\Work\Python\Examples\2-Importing\teachers.xlsx'
import pandas as pd
ExcelReader = pd.ExcelFile(path)
ExcelReader.sheet_names
sheets = ExcelReader.sheet_names
excle.parse()
ExcelReader.parse()
ExcelReader.parse(sheet_name='Sheet1')
ExcelReader.parse(sheet_name=['Sheet1'])
ExcelReader.parse(sheet_name=['Sheet1'], index_col=0)
ExcelReader.parse(sheet_name=['Sheet1'], index_col=0, usecols=1)
ExcelReader.parse(sheet_name=['Sheet1'], index_col=0, usecols=[1])
ExcelReader.parse(sheet_name='Sheet1', index_col=0, usecols=[1])
ExcelReader.parse(sheet_name='Sheet1', index_col=0, usecols=[1, 2])
ExcelReader.parse(sheet_name='Sheet1', index_col=0, usecols=[1, 2], skipfooter=1)
ExcelReader.parse(sheet_name='Sheet1', index_col=0, usecols=[1, 2], skipfooter=1, skiprows=1)
ExcelReader.parse(sheet_name='Sheet1', index_col=0, usecols=[1, 2], 
                  skipfooter=1, skiprows=1, header=0)
ExcelReader.parse(sheet_name='Sheet1', usecols=[1, 2], 
                  skipfooter=1, skiprows=1, names = ['Name', 'Family'])
path = r'H:\Work\Python\Examples\2-Importing\battledeath.xlsx'
ExcelReader = pd.ExcelFile(path)
sheets = ExcelReader.sheet_names
sheets
ExcelReader.parse(sheet_name=0)
ExcelReader.parse(sheet_name=1)
ExcelReader.parse(sheet_name=[0, 1])
ExcelReader.parse(sheet_name=sheets)
ExcelReader.parse(sheet_name=1)
data = ExcelReader.parse(sheet_name=1)
pd.to_csv(r'H:\Work\Python\Examples\2-Importing\battledeath_2024-11-07.csv')
data.to_csv(r'H:\Work\Python\Examples\2-Importing\battledeath_2024-11-07.csv')
path = r'H:\Work\Python\Examples\2-Importing\battledeath_2024-11-07.xlsx'
ExcelWriter = pd.ExcelWriter(path)
data.to_excel(ExcelWriter, sheet_name = 'new')
ExcelWriter.save()
%clear
pd.read_sas(r'H:\Work\Python\Examples\2-Importing\airline.sas7bdat')
pd.read_sas(r'H:\Work\Python\Examples\2-Importing\airline.sas7bdat', index_col = 0)
pd.read_sas(r'H:\Work\Python\Examples\2-Importing\airline.sas7bdat')
data = pd.read_sas(r'H:\Work\Python\Examples\2-Importing\airline.sas7bdat')
data.index(data.Year)
data.index = data.Year
data.Year
data = pd.read_sas(r'H:\Work\Python\Examples\2-Importing\airline.sas7bdat')
data.Year
data
data.columns
data.YEAR
data.index = data.YEAR
data
del data.YEAR
del data['YEAR']
data
pd.read_spss(path)
path = r'H:\Work\Python\Examples\2-Importing\computer.dta'
pd.read_spss(path)
import pandas as pd
path = r'H:\Work\Python\Examples\2-Importing\computer.dta'
pd.read_spss(path)
path = r'H:\Work\Python\Examples\2-Importing\computer.dta'
pd.read_spss(path)
path = r'H:\Work\Python\Examples\2-Importing\trade.dta'
pd.read_spss(path)
path = r'H:\Work\Python\Examples\2-Importing\disarea.dta'
pd.read_spss(path)
import pandas as pd
path = r'H:\Work\Python\Examples\2-Importing\disarea.dta'
pd.read_stata(path)
path = r'H:\Work\R\Examples\2-Importing\6-StatisticalSoftwares\SPSS\international.sav'
pd.read_spss(path)
data.to_sas()
from sas7bdat import SAS7BDAT
from SAS7BDAT import SAS7BDAT
from SAS7BDAT import sas7bdat
import SAS7BDAT
import scipy.io
mat = r'H:\Work\Python\Examples\2-Importing\ja_data2.mat'
path = r'H:\Work\Python\Examples\2-Importing\ja_data2.mat'
mat = scipy.io.matlab.loadmat(path)
mat
mat['cfpCyt']
type(mat['cfpCyt'])
## API
from requests import urlretrive
from Request import urlretrive
from urllib.request import urlretrive
import urllib
from urllib.request import urlretrieve
urlretrieve('https://drive.google.com/uc?id=1zO8ekHWx9U7mrbx_0Hoxxu6od7uxJqWw&export=download')
urlretrieve(url, filename=r'H:\Work\Python\Examples\downloaded.csv')
url = 'https://drive.google.com/uc?id=1zO8ekHWx9U7mrbx_0Hoxxu6od7uxJqWw&export=download'
urlretrieve(url, filename=r'H:\Work\Python\Examples\downloaded.csv')
pd.read_csv(url)
req = Request(url)
from urllib.request import urlretrieve, urlopen, Request
req = Request(url)
req
type(req)
resp = urlopen(req)
resp
resp.read()
import requests
resp = requests.get(url)
requests.get(url)
resp.text
import requests
from bs4 import BeautifulSoup

url = 'https://example.com/'
resp = requests.get(url)
resp.text
html = resp.text
soup = BeautifulSoup(html)
soup
resp.status_code
soup.title
soup.get_text('p')
soup.find_all('a')

url = 'https://www.wikipedia.org/'

resp = requests.get(url)
html = resp.text
# resp.status_code
soup = BeautifulSoup(html)
soup.find_all('a')
result = soup.find_all('a')
type(result)<br>
result[0]<br>
result[1]<br>
result[3]<br>
%clear<br>
[link for link soup.find_all('a')]<br>
[link for link in soup.find_all('a')]<br>
[link.get('href') for link in soup.find_all('a')]<br>
import json<br>
jsonData = '{"name":"John", "age":30, "car":null}'<br>
json.loads(jsonData)<br>
result = json.loads(jsonData)<br>
result['name']<br>
path = r'H:\Work\Python\Examples\2-Importing\cakes.json'<br>
json.load(path)<br>
jsonReader = open(path, 'rt')<br>
json.load(jsonReader)<br>
pd.read_json(jsonReader)<br>
pd.read_json(path)<br>
%clear<br>
url = 'http://www.omdbapi.com/?i=tt3896198&apikey=4fd5103f'<br>
requests.get(utl + '&t=batman+the+dark+knight')<br>
requests.get(url + '&t=batman+the+dark+knight')<br>
resp = requests.get(url + '&t=batman+the+dark+knight')<br>
resp<br>
resp.text<br>
resp.json()<br>
result = resp.json()<br>
result['Year']<br>

## ---(Fri Nov  8 14:03:00 2024)---<br>
# ORM<br>
import sqlalchemy as sa<br>
con = 'mssql+pyodbc://sa:1234@SB2\MSSQLSERVER19TAB/AdventureWorksDW2020?driver=SQL+Server+Native+Client+11.0'<br>
engine = sa.create_engine(con)<br>
connection= engine.connect()<br>
stmt = sa.text('select * from DimAccount')<br>
stmt<br>
proxy = connection.execute(stmt)<br>
proxy<br>
proxy.fetchall()<br>
proxy = connection.execute(stmt)<br>
results= proxy.fetchall()<br>
results<br>
stmt = sa.text('select * from FactCallCenter')<br>
proxy = connection.execute(stmt)<br>
proxy.fetchall()<br>
from sqlalchemy import Inspector<br>
sa.Inspector()<br>
import pandas as pd<br>
pd.read_sql(stmt, connection)<br>
df = pd.read_sql(stmt, connection)<br>
import sqlalchemy as sa<br>
from sqlalchemy import Inspector<br>
con = 'mssql+pyodbc://sa:1234@SB2\MSSQLSERVER19TAB/AdventureWorksDW2020?driver=SQL+Server+Native+Client+11.0'<br>
engine = sa.create_engine(con)<br>
metadata = sa.MetaData()<br>
metadata<br>
address = sa.Table('New', metadata, schema = 'dbo', autoload=True, autoload_with=engine)<br>
sa.inspect()<br>
sa.inspector.get_table_names()<br>
sa.inspect()<br>
sa.inspect(engine)<br>
sa.inspect(engine).get_table_names()<br>
import pandas.io.sql<br>
import pyodbc<br>

"""
Created on Fri Nov  8 14:20:24 2024<br>

@author: ali sadeghi aghili<br>
"""

import pandas.io.sql<br>
import pyodbc<br>

# Parameters<br>
server = 'SB2\MSSQLSERVER19TAB'<br>
db = 'AdventureWorksDW2020'<br>
#port=...<br>
#user=...<br>
#pass=...<br>

# Create the connection<br>
conn = pyodbc.connect('DRIVER={SQL Server};SERVER=' + server + ';DATABASE=' + db + ';Trusted_Connection=yes')<br>
sql = """<br>
select * from [dbo].[FactCallCenter]<br>
"""<br>
df = pandas.io.sql.read_sql(sql, conn)<br>
df<br>
df.to_sql('new', conn)<br>
# pandas prefers an SQLAlchemy engine or connection, not a raw pyodbc connection<br>
df.to_sql('new', con)<br>
khoraki = ['pofak', 'chips', 'shokolat', 'chips', 'adams', 'lavashak', 'pofak', 'choob shoor']<br>
set(khoraki)<br>
khorakiSet = set(khoraki)<br>
khorakiSet.add('pashmak')
khorakiSet
khorakiSet.add('pashmak')
khorakiSet
khorakiSet.add('pofak')
khorakiSet
khorakiSet.update(['chips', 'maste moosir', 'pastil'])
khorakiSet
khorakiSet.pop()
khorakiSet.discard('pashmak')
khorakiSet
khorakiSet.discard('pashmak')
khorakiSet.discard('pastil')<br>
khorakiSet<br>
khorakiSet.discard('pastil')<br>
aliAte = ['pofak', 'chips', 'adams']<br>
hassanAte = ['chips', 'mast moosir', 'pofak']<br>
aliAte.union(hassanAte)<br>
aliAte = set(['pofak', 'chips', 'adams'])<br>
hassanAte = set(['chips', 'mast moosir', 'pofak'])<br>
aliAte.union(hassanAte)<br>
runcell(0, 'C:/Users/alisa/untitled3.py')<br>
aliAte.intersection(hassanAte)<br>
hassanAte.intersection(aliAte)<br>
aliAte<br>
aliAte.difference(hassanAte)<br>
hassanAte.difference(aliAte)<br>
%clear<br>
# defaultdict<br>
{'key':'value'}
statesDict = {}
for state, city in city_list:
    if state not in statesDict:
        statesDict[state] = city
    else:
        statesDict[state].apend(city)
city_list = [('TX','Austin'), ('TX','Houston'), ('NY','Albany'), 
             ('NY', 'Syracuse'), ('NY', 'Buffalo'), ('NY', 'Rochester'), 
             ('TX', 'Dallas'), ('CA','Sacramento'), ('CA', 'Palo Alto'), 
             ('GA', 'Atlanta')]

statesDict = {}
for state, city in city_list:
    if state not in statesDict:
        statesDict[state] = city
    else:
        statesDict[state].apend(city)
city_list = [('TX','Austin'), ('TX','Houston'), ('NY','Albany'), 
             ('NY', 'Syracuse'), ('NY', 'Buffalo'), ('NY', 'Rochester'), 
             ('TX', 'Dallas'), ('CA','Sacramento'), ('CA', 'Palo Alto'), 
             ('GA', 'Atlanta')]

statesDict = {}
for state, city in city_list:
    if state not in statesDict:
        statesDict[state] = city
    else:
        statesDict[state].append(city)
statesDict = {}
for state, city in city_list:
    if state not in statesDict:
        statesDict[state] = [city]
    else:
        statesDict[state].append(city)
statesDict
from collections import defaultdict
statesDict2 = defaultdict(list)
statesDict = {}
for state, city in city_list:
    if state not in statesDict:
        statesDict[state] = []
    statesDict[state].append(city)
statesDict
for state, city in city_list:
    statesDict[state].append(city)
for state, city in city_list:
    statesDict2[state].append(city)
statesDict = {}
for state, city in city_list:
    if state not in statesDict:
        statesDict[state] = []
    statesDict[state].append(city)
statesDict
statesDict2
statesDict2['TX']
tweets = pd.read_csv(r'H:\Work\Python\Examples\1-basics\tweets.csv', usecols='lang')
tweets
tweets = pd.read_csv(r'H:\Work\Python\Examples\1-basics\tweets.csv', usecols='Lang')
tweets = pd.read_csv(r'H:\Work\Python\Examples\1-basics\tweets.csv', usecols=['Lang'])
tweets = pd.read_csv(r'H:\Work\Python\Examples\1-basics\tweets.csv', usecols=['lang'])
tweets
tweets.lang
langDict = {}
for lang in tweets.lang:
    if lang not in langDict:
        langDict[lang] = 1
    else:
        langDict[lang] += 1
langDict
from collections import Counter
Counter(tweets.lang)
Counter(tweets.lang).most_common(1)
Counter(tweets.lang).most_common(2)
bday = '1988/08/27'
type(bday)
datetime.strptime(bday, '%Y/%m/%d')
from datetime import datetime
bday = '1988/08/27'
datetime.strptime(bday, '%Y/%m/%d')
dates = ['02/19/2001',
 '04/10/2001',
 '05/30/2001',
 '07/19/2001',
 '09/07/2001',
 '10/27/2001',
 '12/16/2001',
 '02/04/2002',
 '03/26/2002',
 '05/15/2002',
 '07/04/2002',
 '08/23/2002',
 '10/12/2002',
 '12/01/2002',
 '01/20/2003',
 '03/11/2003',
 '04/30/2003',
 '06/19/2003',
 '08/08/2003',
 '09/27/2003',
 '11/16/2003',
 '01/05/2004',
 '02/24/2004',
 '04/14/2004',
 '06/03/2004',
 '07/23/2004',
 '09/11/2004',
 '10/31/2004',
 '12/20/2004',
 '02/08/2005',
 '03/30/2005',
 '05/19/2005',
 '07/08/2005',
 '08/27/2005',
 '10/16/2005',
 '12/05/2005',
 '01/24/2006',
 '03/15/2006',
 '05/04/2006',
 '06/23/2006',
 '08/12/2006',
 '10/01/2006',
 '11/20/2006',
 '01/09/2007',
 '02/28/2007',
 '04/19/2007',
 '06/08/2007',
 '07/28/2007',
 '09/16/2007',
 '11/05/2007',
 '12/25/2007',
 '02/13/2008',
 '04/03/2008',
 '05/23/2008',
 '07/12/2008',
 '08/31/2008',
 '10/20/2008',
 '12/09/2008',
 '01/28/2009',
 '03/19/2009',
 '05/08/2009',
 '06/27/2009',
 '08/16/2009',
 '10/05/2009',
 '11/24/2009',
 '01/13/2010',
 '03/04/2010',
 '04/23/2010',
 '06/12/2010',
 '08/01/2010',
 '09/20/2010',
 '11/09/2010',
 '12/29/2010',
 '02/17/2011',
 '04/08/2011',
 '05/28/2011',
 '07/17/2011',
 '09/05/2011',
 '10/24/2011',
 '11/12/2011',
 '01/01/2012',
 '02/20/2012',
 '04/10/2012',
 '05/30/2012',
 '07/19/2012',
 '09/07/2012',
 '10/27/2012',
 '12/16/2012',
 '02/04/2013',
 '03/26/2013',
 '05/15/2013',
 '07/04/2013',
 '08/23/2013',
 '10/12/2013',
 '12/01/2013',
 '01/20/2014',
 '03/11/2014',
 '04/30/2014',
 '06/19/2014',
 '08/08/2014',
 '09/27/2014',
 '11/16/2014',
 '07/05/2014',
 '01/24/2015',
 '03/15/2015',
 '05/04/2015',
 '06/23/2015',
 '08/12/2015',
 '10/01/2015',
 '11/20/2015',
 '01/09/2016',
 '02/28/2016',
 '04/18/2016',
 '06/07/2016',
 '07/27/2016',
 '09/15/2016',
 '11/04/2016']
datetime.strptime(bday, '%Y-%m/%d')<br>
bday = '1988-08/27'<br>
datetime.strptime(bday, '%Y-%m/%d')<br>
bday = '1988 08/27'<br>
datetime.strptime(bday, '%Y %m/%d')<br>
date<br>
dates<br>
[datetime.strptime(date, '%m/%d/%Y') for date in dates]<br>
dated = [datetime.strptime(date, '%m/%d/%Y') for date in dates]<br>
dated<br>
bdayDated = datetime.strptime(bday, '%Y %m/%d')<br>
bdayDated<br>
datetime.strftime(bdayDated, '%B')<br>
datetime.strftime(bdayDated, '%B %d')<br>
datetime.strftime(bdayDated, '%B %d, %Y')<br>
datetime.strftime(bdayDated, '%A')<br>
%clear<br>
bdayDated<br>
# TimeZone naive<br>
bdayDated.year<br>
bdayDated.month<br>
bdayDated.hour<br>
bdayDated.tzinfo
datetime.now()
now = datetime.now()
now
datetime.utcnow()
%clear
import pytz
pytz.all_timezones
len(pytz.all_timezones)
now
now.tzinfo
# localize
zone = pytz.timezone('Iran')
zone
zone.localize(now)
now
now = zone.localize(now)
now
now.tzinfo
bdayDated
bdayDated = zone.localize(bdayDated)
bdayDated
now
now.astimezone(pytz.timezone('Asia/Istanbul'))
now.astimezone(pytz.timezone('Japan'))
now.tzinfo
now
now.replace(year = 2023)
now.replace(tzinfo = pytz.timezone('Japan'))
# time delta
from datetime import datetime, timedelta
now - bdayDated
# epoch
# 1970-01-01
now
now.replace(year = 2025)
now + timedelta(days = 365)
[now + timedelta(days = day) for day in range(366)]
pytz.all_timezones
now - bdayDated
now + timedelta(days = 365)
# datetime manipultion
# string manipulation
# Regular Expressions
# NLP: Natural Language Processing
%clear
import re
text = '''101 COM Computer
205 MAT Mathematics
189 ENG English'''
newLine = re.complie(pattern = '\n')
spaces = re.complie(pattern = '\s+')
newLine = re.compile(pattern = '\n')
spaces = re.compile(pattern = '\s+')
newLine
spaces
re.split(pattern=newLine, string=text)
re.split(pattern=spaces, string=text)
re.split(pattern=r'\n', string=text)
re.findall(pattern = r'\d+', string = text)
re.search(pattern = r'\d+', string = text)
result = re.search(pattern = r'\d+', string = text)
result.group()
result.start()
result.end()
result.span()
# greedy
re.search(pattern = r'\d+', string = text)
re.match(pattern = r'\d+', string = text)
re.search(pattern = r'\n+', string = text)
re.match(pattern = r'\n+', string = text)
# ^\d+
# \d+
# ^\n+
re.match(pattern = r'\n+', string = text)
# \n+
re.search(pattern = r'\n+', string = text)
re.sub(pattern=r'(?!\n)\s', repl='\t', string=text)
from sys import stdout
stdout.write(re.sub(pattern=r'(?!\n)\s', repl='\t', string=text))
pattern = re.compile(r'\d+\s[A-Z]{3}\s[A-Z][a-z]+')
re.findall(pattern, string = text)
pattern = re.compile(r'(\d+)\s([A-Z]{3})\s([A-Z][a-z]+)')
re.findall(pattern, string = text)
re.findall(pattern, string = text).group()
re.search(pattern, string = text).group()
re.search(pattern, string = text).group(0)
re.search(pattern, string = text).group(1)
re.search(pattern, string = text).group(2)
re.search(pattern, string = text).group(3)
sentence = 'ali dar dar jahad daneshgahi daneshgahi tadris mi konad konad'
re.search(pattern, string = text).group(0)
re.search(pattern, string = text).group(1)
re.search(pattern, string = text).group(2)
re.search(pattern, string = text).group(3)<br>
re.sub(string=sentence, pattern = r'(\w+)\s\1', repl = '\g<1>')<br>
re.sub(string=sentence, pattern = r'(\w{2,})\s\1', repl = '\g<1>')<br>
## pivot & unpivot(melt)
pd.read_excel(r'H:\Work\Python\Examples\3-Cleansing\CrossTable.xlsx')<br>
df = pd.read_excel(r'H:\Work\Python\Examples\3-Cleansing\CrossTable.xlsx')<br>
df.melt(id_vars = 'Product', var_name='MonthYear', value_name = 'Sell')<br>
melted = df.melt(id_vars = 'Product', var_name='MonthYear', value_name = 'Sell')<br>
melted.pivot(index='Product', columns = 'MonthYear', values = 'Sell')<br>
%clear<br>
melted<br>
melted.MonthYear<br>
re.split(pattern=\s, string=melted.MonthYear)<br>
re.split(pattern='\s', string=melted.MonthYear)<br>
[re.split(pattern='\s', string=MonthYear) for MonthYear in melted.MonthYear]<br>
'ali sadeghi'.split(' ')<br>
melted.MonthYear.str.split(' ')<br>
a, b = melted.MonthYear.str.split(' ')<br>
melted.MonthYear.str.split(' ').get(0)<br>
melted.MonthYear.str.split(' ').str.get(0)<br>
melted.MonthYear.str.split(' ')<br>
melted.MonthYear.str.split(' ').str.get(0)<br>
melted['Month'] = melted.MonthYear.str.split(' ').str.get(0)<br>
melted<br>
melted['Year'] = melted.MonthYear.str.split(' ').str.get(1)<br>
melted<br>
[Year + '-' + Month for Month, Year in zip(melted.Month, melted.Year)]<br>
melted['YearMonth ']= [Year + '-' + Month for Month, Year in zip(melted.Month, melted.Year)]<br>
del melted['YearMonth ']<br>
melted['YearMonth']= [Year + '-' + Month for Month, Year in zip(melted.Month, melted.Year)]<br>
melted<br>
melted['YearMonth']= [Year + '-' + Month for Month, Year in zip(melted.Month, melted.Year)]<br>
songs = pd.read_csv(r'H:\Work\Python\Examples\5-Manipulation\stage_songs.csv')<br>
writers = pd.read_csv(r'H:\Work\Python\Examples\5-Manipulation\stage_writers.csv')<br>
songs<br>
writers<br>
song.merge(writers, left_on = 'Music', right_on = 'song', how = 'inner')<br>
songs.merge(writers, left_on = 'Music', right_on = 'song', how = 'inner')<br>
result = songs.merge(writers, left_on = 'Music', right_on = 'song', how = 'inner')<br>










