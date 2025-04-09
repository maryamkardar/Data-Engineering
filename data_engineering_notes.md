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








