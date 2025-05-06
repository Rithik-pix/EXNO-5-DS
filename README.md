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
 import pandas as pd
 import numpy as np
 import seaborn as sns
 import matplotlib.pyplot as plt
 x = [1, 2, 3, 4, 5]
 y = [3, 6, 2, 7, 1]
 plt.plot(x,y,label='line1')
```

![image](https://github.com/user-attachments/assets/53e117fb-6bee-4d45-bf80-c8fd8254f164)

```
x1 = [1,2,3]
y1 = [2,4,1]
x2 = [1,2,3]
y2 = [4,1,3]
plt.plot(x1,y1,label='line1')
plt.plot(x2,y2,label='line2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph!')
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/d8d56c02-50a1-4eb8-ac54-914476309f18)

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

![image](https://github.com/user-attachments/assets/90a36295-e2ba-467f-9219-2b41bcfada39)

```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)

```

![image](https://github.com/user-attachments/assets/7e994ea8-d55a-4093-8fff-c195a13e234e)



```
years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
```

![image](https://github.com/user-attachments/assets/b503922b-cad5-4bf5-af1e-a3b79c4799c6)

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

![image](https://github.com/user-attachments/assets/ace63430-31e3-4447-a35d-f19716a15ada)

```
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yield of Oranges (tons per hectare)");
```

![image](https://github.com/user-attachments/assets/1aed0b97-a2d2-426c-9544-b41a261f4cb0)

```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
# The following lines were indented but shouldn't be. 
# Removed the indentation to fix the issue.
x # array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])
y # array([11, 12, 13, 14, 15, 16, 17, 18, 19, 20])
plt.scatter(x,y,c='r')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```

![image](https://github.com/user-attachments/assets/b9309850-70e4-44ee-8109-0fdf34c11fa8)

```
y=x*x
y
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
plt.legend(['y-values']);

```

![image](https://github.com/user-attachments/assets/37e18995-5ff1-43dc-8c5a-4ef5e243b62d)


```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
```

![image](https://github.com/user-attachments/assets/2b353e9f-6dd6-478a-83df-9037fda93246)

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

![image](https://github.com/user-attachments/assets/f9411128-9ebe-4be2-bf8e-dcfde9687648)

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

![image](https://github.com/user-attachments/assets/73a1f50e-079b-4138-98c8-2a27112c7708)

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
![image](https://github.com/user-attachments/assets/01fa7065-a76a-4d53-9781-316867dc27b8)


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

![image](https://github.com/user-attachments/assets/21e32708-216b-4d37-814f-ae60b091cf03)

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

![image](https://github.com/user-attachments/assets/228b60d4-e16b-49a2-8908-ba9d2a765e5d)

```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```

![image](https://github.com/user-attachments/assets/654aa475-b9c9-4596-8d50-044b7c212c86)

```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```


![image](https://github.com/user-attachments/assets/34c1b61b-d60d-42dc-a9ec-a09fc3481322)

```
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```

![image](https://github.com/user-attachments/assets/e3fa12a9-9945-4661-9471-e2b1f0b91050)

```
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=
['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
```

![image](https://github.com/user-attachments/assets/efeb79cb-a631-46d5-a35f-768c5577b62b)

# Result:
 To Perform Data Visualization using matplot python library for the given datas is successful.
