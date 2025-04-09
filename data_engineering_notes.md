Data Processing with Python

First Session:🙌

print("your BMI is:",{BMI})
print(f"your BMI is: {BMI}")
print('your BMI is:' + str(BMI))
print("your BMI", BMI, sep= ":")

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














