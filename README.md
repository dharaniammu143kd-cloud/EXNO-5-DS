# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
```
```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd

x = [2018, 2019, 2020, 2021, 2022]
y = [15000, 20000, 25000, 30000, 35000]

plt.plot(x, y, 'g*', linestyle='dashed', linewidth=2, markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('2D Diagram')
plt.show()
```

<img width="652" height="455" alt="image" src="https://github.com/user-attachments/assets/9bea77bb-0695-4130-bddb-47135b2b2a97" />

```
plt.subplot(2,2,1)
plt.plot(x,y,'--')
plt.subplot(2,2,2)
plt.plot(x,y,'o--')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
plt.show()
```

<img width="745" height="502" alt="image" src="https://github.com/user-attachments/assets/e2caec5a-e123-4c22-8c4d-778b93570fb7" />

```
x = np.arange(0, 4*np.pi, 0.1)
y = np.sin(x)
plt.title("sine waveform")
plt.plot(x,y)
plt.show()
```

<img width="666" height="460" alt="image" src="https://github.com/user-attachments/assets/f61f9746-020c-4170-8f44-388c9c10dab2" />

```
x = [2, 8, 10]
y = [11, 16, 9]
x1 = [3, 4, 11] 
y1 = [6, 15, 7]
plt.bar(x, y, color='r')
plt.bar(x1, y1, color='g')
plt.title("Bar graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```

<img width="712" height="479" alt="image" src="https://github.com/user-attachments/assets/5a2bb478-373a-460a-971a-80463a037145" />

```
x = [1, 2, 3]
y = [7, 3, 9]

plt.plot(x, y, color='g')
plt.title("line graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```

<img width="789" height="537" alt="image" src="https://github.com/user-attachments/assets/bcddcbcf-2474-47ea-beef-7aecd1580804" />

```
x1 = [1, 2, 3]
y1 = [2, 4, 1]
plt.plot(x1, y1, label='line1')

x2 = [1, 2, 3]  
y2 = [4, 1, 3]
plt.plot(x2, y2, label='line2')

plt.title("multiline graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```

<img width="665" height="483" alt="image" src="https://github.com/user-attachments/assets/fe647efd-8e2d-4e0d-87c3-f86b4bfc78f4" />

```
x = [1, 2, 3, 4, 5, 6]
y = [2, 4, 1, 5, 2, 6]
plt.plot(x, y, color='green', linestyle='dashed', linewidth=3, 
         marker='o', markerfacecolor='red', markersize=12, label='spices')
plt.xlim(1, 8)
plt.ylim(1, 8) 
plt.title("line graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```

<img width="682" height="501" alt="image" src="https://github.com/user-attachments/assets/530358dc-d60b-4518-b18d-cd6ded175b1c" />

```
yield_apples=[0.895,0.91,0.919,0.926,0.931]
plt.plot(yield_apples,linestyle='dashed',linewidth=3,marker='*',markersize=12,color='g')
plt.show()
```

<img width="626" height="430" alt="image" src="https://github.com/user-attachments/assets/6d222522-bdcd-413b-9ded-bc1fc1e9f983" />

```
oranges = [2, 4, 6, 7, 8, 12, 45]
apples = [2, 4, 5, 6, 8, 23, 37]
years = [2019, 2020, 2021, 2022, 2023, 2024, 2025]
plt.plot(years, apples, marker='o')
plt.plot(years, oranges, marker='*')
plt.title('Crop yields in Kanto')
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.legend(['apples', 'oranges'])  
plt.show()
```

<img width="737" height="559" alt="image" src="https://github.com/user-attachments/assets/870a9871-1530-4af4-aeb2-8c644dfbfcea" />

```
oranges = [2, 4, 6, 7, 8, 12]
apples = [2, 4, 5, 6, 8, 23]
years = [2019, 2020, 2021, 2022, 2023, 2024]
plt.bar(oranges,apples)
plt.plot(years, apples, label='apples', marker='*')
plt.plot(years, oranges, label='oranges', marker='o')
plt.title('Fruit sales')  
plt.xlabel('Year')  
plt.ylabel('Sales')  
plt.legend()  
plt.show()
```

<img width="758" height="528" alt="image" src="https://github.com/user-attachments/assets/8aa84a98-94fc-4cfc-bb42-5e365559f7c9" />

```
plt.figure(figsize=(12,6))
plt.plot(years, oranges, marker='o',label='oranges')
plt.title("yield of oranges (tons per hectare)")
plt.legend()
```

<img width="813" height="437" alt="image" src="https://github.com/user-attachments/assets/151339f4-d1ea-4b20-88c9-0924bf082f10" />

```
import matplotlib.pyplot as plt
print("scatter plot is:")
x = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
y = [2, 4, 5, 7, 6, 8, 9, 11, 12, 12]
plt.scatter(x, y, label='star', color='green', marker='*', s=30)
plt.title("my scatterplot!")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```

<img width="689" height="498" alt="image" src="https://github.com/user-attachments/assets/fc33fbce-6a06-45e2-9df4-a2142a948169" />

```
import matplotlib.pyplot as plt
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5, 7, 9, 11, 13]
y3 = [2, 4, 6, 8, 10]
plt.fill_between(x, y1, color='green',label='y1')
plt.fill_between(x, y2, color='blue', label='y2')
plt.fill_between(x, y3, color='red',label='y3')
plt.title("Fill Between Example")
plt.legend()
plt.show()
```

<img width="692" height="539" alt="image" src="https://github.com/user-attachments/assets/6eb31b26-65c9-4457-af56-3726192d066b" />

```
plt.stackplot(x,y1,y2,y3,labels=['line1','line2','line3'])
plt.legend(loc='upper left')
plt.title("Stacked line chart")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```

<img width="643" height="514" alt="image" src="https://github.com/user-attachments/assets/6907bbfc-1839-4760-a7c5-e62c3e043011" />

```
from scipy.interpolate import make_interp_spline
x = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
y = np.array([2, 4, 5, 7, 8, 9, 10, 11, 12, 13])
spl = make_interp_spline(x, y)
x_smooth = np.linspace(x.min(), x.max(), 100)
y_smooth = spl(x_smooth)
plt.plot(x, y, 'o', label='data')
plt.plot(x_smooth, y_smooth, '-', label='spline')
plt.legend()
plt.show()
```

<img width="726" height="557" alt="image" src="https://github.com/user-attachments/assets/879b5ba7-87cc-4c38-a965-30b1e7b89373" />

```
values=[5,6,7,3,2]
names=['A','B','C','D','E']
plt.bar(names,values,color='green')
plt.show()
```

<img width="696" height="471" alt="image" src="https://github.com/user-attachments/assets/762c0288-ee40-49e1-8bb3-8c9365fc0a94" />

```
ages = [2, 5, 70, 40, 45, 50, 43, 40, 44, 60, 7, 13, 57, 18, 90, 77, 32, 21, 20, 40]
range1 = (0, 100)
bins = 10
plt.hist(ages, bins, range1, color='green', histtype='bar', rwidth=0.8)
plt.xlabel('ages')
plt.ylabel('no. of people')
plt.title('my histogram')
plt.show()
```

<img width="645" height="552" alt="image" src="https://github.com/user-attachments/assets/fd1c5656-9f00-491e-bb6e-b897b8691e88" />

```
x=[2,1,6,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x,bins=10,color='green',alpha=0.5)
plt.show()
```

<img width="732" height="542" alt="image" src="https://github.com/user-attachments/assets/01ae2c8a-6145-4340-996f-74a17681fdc3" />

```
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```

<img width="669" height="426" alt="image" src="https://github.com/user-attachments/assets/77f52c8a-041b-4de6-9490-88e25685e5f5" />

```
fig, ax = plt.subplots()
ax.boxplot(data)
ax.set_xlabel('x-axis')
ax.set_ylabel('y-axis')
ax.set_title('box plot')
```

<img width="734" height="580" alt="image" src="https://github.com/user-attachments/assets/065cbcea-0689-4b52-837d-1af6eddaf89d" />

```
activities=['eat', 'sleep', 'work', 'play']
slices=[3,7,8,6]
colors=['y', 'g', 'b', 'r']
plt.pie(slices, labels=activities, colors=colors, startangle=90, shadow=True, explode=(0,0,0.1,0), radius=1.2, autopct="X1.1")
plt.legend()
plt.show()
```

<img width="469" height="376" alt="image" src="https://github.com/user-attachments/assets/f3ad2984-922b-4cb3-addd-684cb338d823" />

```
labels='python', 'C+', 'ruby', 'java'
sizes=[215,130,245,210]
colors=['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes, explode=explode, colors=colors, labels=labels, autopct='%1.1f%%', shadow=True)
plt.axis('equal')
plt.show()
```

<img width="536" height="433" alt="image" src="https://github.com/user-attachments/assets/cc891b65-c075-4324-94c9-68467317c44b" />

# Result:
 
Thus,all the data visualization techniques of matplotlib has been implemented
