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
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label='line1')
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label='line2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph!')
plt.legend()
plt.show()
```

![Screenshot 2024-11-11 083850](https://github.com/user-attachments/assets/85a37301-878a-47c5-b42e-d9cc2b5e7bb7)

```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations!')
plt.show()
```

![Screenshot 2024-11-11 083924](https://github.com/user-attachments/assets/ae3f0c37-c141-44a2-8019-35d9830b856e)

```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```

![Screenshot 2024-11-11 083959](https://github.com/user-attachments/assets/5d9c7080-7743-4900-b114-34d73265989c)

```
years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
```

![Screenshot 2024-11-11 084043](https://github.com/user-attachments/assets/de73eb07-aa73-4cb2-81c2-a993e8cbb4e0)

```
years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.926,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896, ]
plt.plot(years, apples)
plt.plot(years, oranges)
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title('Crop Yields in Kanto')
plt.legend(['Apples','Oranges']);
```

![Screenshot 2024-11-11 084122](https://github.com/user-attachments/assets/8bdc1268-4fe6-4f4e-b643-838a53eed3db)

```
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yield of Oranges (tons per hectare)");
```

![Screenshot 2024-11-11 084155](https://github.com/user-attachments/assets/7c489155-06df-4170-854b-674db555b9c3)

```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x
```

![Screenshot 2024-11-11 084549](https://github.com/user-attachments/assets/6ca841f9-1c3a-43cf-81a9-35c6c6e96ff8)

```
y
```

![Screenshot 2024-11-11 084558](https://github.com/user-attachments/assets/66d971c9-cd76-4df3-afef-6ec33a146842)

```
plt.scatter(x,y,c='r')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```

![Screenshot 2024-11-11 084612](https://github.com/user-attachments/assets/164a2391-5d02-4720-aa84-52731a8ffb28)

```
y=x*x
y
```

![Screenshot 2024-11-11 084622](https://github.com/user-attachments/assets/fa0b7ff7-093f-4edb-86c8-66f72ef51b7c)

```
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
```

![Screenshot 2024-11-11 084629](https://github.com/user-attachments/assets/8049971b-963f-4f79-826e-08bd892db6aa)

```
np.pi
```

![Screenshot 2024-11-11 084636](https://github.com/user-attachments/assets/00587a76-60e5-49f5-92d7-5f1fcd6fd0a2)

```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
```

![Screenshot 2024-11-11 084647](https://github.com/user-attachments/assets/6518b0e3-8e07-4a33-b4b0-a2582a0eea7d)

```
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
```

![Screenshot 2024-11-11 084653](https://github.com/user-attachments/assets/c801e27a-11b2-4d1e-bc86-637b7d4b95b6)

```
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')

plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')
plt.legend(['y1','y2'])
plt.show()
```

![Screenshot 2024-11-11 084700](https://github.com/user-attachments/assets/611dcbc8-be1d-4ac2-81b0-65df6af6115d)

```
import matplotlib.pyplot as plt
height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['red','green']
c2=['b','g']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My bar chart!')
plt.show()
```

![Screenshot 2024-11-11 084706](https://github.com/user-attachments/assets/08dd937a-cbef-4dc4-b4d6-03a6094672ec)

```
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show()
```

![Screenshot 2024-11-11 084719](https://github.com/user-attachments/assets/1f3b9893-23ee-4fc1-95a3-3a82b185fbac)

```
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No. of people')
plt.title('My histogram')
plt.show()
```

![Screenshot 2024-11-11 084728](https://github.com/user-attachments/assets/08a658c2-64d5-4c0e-a7c9-8a05f1863076)

```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```

![Screenshot 2024-11-11 084736](https://github.com/user-attachments/assets/9735305e-3d20-47fb-b114-572ed913079e)

```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```

![Screenshot 2024-11-11 084745](https://github.com/user-attachments/assets/1307b6a2-40ff-48d9-aff0-811e513c92c4)

```
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```

![Screenshot 2024-11-11 084751](https://github.com/user-attachments/assets/1bb1b7a2-7f4b-48dc-b0a8-a27eb22e952f)

```
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
```

![Screenshot 2024-11-11 084802](https://github.com/user-attachments/assets/25498fc8-b447-4bef-961a-3895d98e66b6)

# Result:
Thus, the implementation of data visualisation using matplotlib has been successfully verified.
