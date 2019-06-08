____________________________

Day 10:Lecture 1
Content: Extended Slicing
Author:Ravishankar Chavare
Date:08-06-2019
LinkedIn:https://www.linkedin.com/in/ravishankar-chavare-84474a102
_______________________________

*Extended Slicing On List*
- Ever since Python 1.4, the slicing syntax has supported an optional third ``step'' or ``stride'' argument

Syntax:
Listname[startindex:endindex:step]

Other valid syntax are

#start list from 0 index

Listname[:endindex:step]

#here start from 0 index and end at last element with given step

Listname[::step]

#here start from startindex index and end at last element with given step

Listname[startindex::step]


- *s[i:j:k]* is
"slice of s from i to j with step k".

When i and jare absent, the whole sequence is assumed and

thus s[::k] means "every k-th item".


Examples:

How to print 2,4,6 

lists=[0,1,2,3,4,5,6,7,8,9]
start=2
end=8
step=2
result=lists[start:end:step]
print(result) 
#Result : [2,4,6]


- lists[::n] is a sequence of each n-th item in the entire sequence.

- [::3] just means that you have not specified any start or end indices for your slice. Since you have specified a step, 3, this will take every third entry of something starting at the first index. For example:

lists=[0,1,2,3,4,5,6,7,8,9]
result=lists[::3]
print(result) 
#Result:[0, 6,9]

Let's take every 3rd item from second position list

lists=[0,1,2,3,4,5,6,7,8,9]
result=lists[2::3]
print(result) 
#Result:[2,5,8]