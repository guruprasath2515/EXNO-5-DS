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
```py
 import pandas as pd
 import numpy as np
 import seaborn as sns
 import matplotlib.pyplot as plt
 x = [1, 2, 3, 4, 5]
 y = [3, 6, 2, 7, 1]
 plt.plot(x,y,label='line1')
```
![image](https://github.com/user-attachments/assets/ea294327-61e7-4d4d-8994-3f78edb7a650)

```py
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
![image](https://github.com/user-attachments/assets/24957f74-fc3b-4705-a899-9001c43d3a0f)

```py
 x=[1,2,3,4,5,6]
 y=[2,4,1,5,2,6]
 plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
 plt.xlabel('x-axis')
 plt.ylabel('y-axis')
 plt.title('Some cool customizations!')
```
![image](https://github.com/user-attachments/assets/b7c4a9a3-68ba-4818-ad8c-20892137efaf)

```py
 yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
 plt.plot(yield_apples)
```
![image](https://github.com/user-attachments/assets/92b39cb2-b848-4dc0-94a2-7a56a2a4d182)

```py
 years=[2010,2011,2012,2013,2014,2015]
 plt.plot(years,yield_apples)
```
![image](https://github.com/user-attachments/assets/e7698d8f-bbfc-48e4-b2c3-cf5bff2d9b65)

```py
 years=range(2000,2012)
 apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
 oranges=[0.926,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896]
 plt.plot(years, apples)
 plt.plot(years, oranges)
 plt.xlabel('Year')
 plt.ylabel('Yield (tons per hectare)')
 plt.title('Crop Yields in Kanto')
 plt.legend(['Apples','Oranges']);
```
![image](https://github.com/user-attachments/assets/6ab38497-feec-4e76-a5e8-10ac3c709262)

```py
 plt.figure(figsize=(12,6))
 plt.plot(years,oranges,marker='o')
 plt.title("Yield of Oranges (tons per hectare)");
```
![image](https://github.com/user-attachments/assets/3c73542e-6e9d-49f2-af82-3d21777a5372)

```py
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 x=np.arange(0,10)
 y=np.arange(11,21)
 x
```
![image](https://github.com/user-attachments/assets/4aff6de4-7e23-435e-af5e-31bb12ea8e89)

```py
y
```
![image](https://github.com/user-attachments/assets/e88750c1-7c83-44be-a808-3725031df454)

```py
 plt.scatter(x,y,c='r')
 plt.xlabel('X-axis')
 plt.ylabel('Y-axis')
 plt.title('Graph in 2D')
 plt.savefig('Test.png')
```
![image](https://github.com/user-attachments/assets/d54bb904-47e7-4227-b056-c5523f9b1936)

```py
y=x*x
y
```
![image](https://github.com/user-attachments/assets/c2985742-f7ee-4cb9-9afc-f43508ac60c3)

```py
 plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
 plt.xlabel('X axis')
 plt.ylabel('Y axis')
 plt.title('2d Diagram')
 plt.legend(['y-values']);
```
![image](https://github.com/user-attachments/assets/9f6e2baf-8556-4edd-86e1-89ea7aa9d875)

```py
 x=np.arange(0,4*np.pi,0.1)
 y=np.sin(x)
 plt.title("sine wave form")
 plt.plot(x,y)
 plt.show()
```
![image](https://github.com/user-attachments/assets/dc354db9-5219-4666-908f-cc593fb0b03c)

```py
 import matplotlib.pyplot as plt
 import numpy as np
 x=[1,2,3,4,5]
 y1=[10,12,14,16,18]
 y2=[5,7,9,11,13]
 y3=[2,4,6,8,10]
 plt.fill_between(x,y1,color='blue')
 plt.fill_between(x,y2,color='green')
```
![image](https://github.com/user-attachments/assets/59485882-e8e1-48ce-a1a2-5500a269cc3b)

```py
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
![image](https://github.com/user-attachments/assets/e0677eea-102d-4ac8-9b3a-2ec2a49253f7)

```py
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
![image](https://github.com/user-attachments/assets/88518162-df6d-4209-ae61-9e57c15d970d)

```py
 ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
 range=(0,100)
 bins=10
 plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
 plt.xlabel('age')
 plt.ylabel('No. of people')
 plt.title('My histogram')
 plt.show()
```
![image](https://github.com/user-attachments/assets/b16eb5bc-621b-45a8-b0bf-20f9482c8bd9)

```py
 np.random.seed(0)
 data=np.random.normal(loc=0,scale=1,size=100)
 data
```
 np.random.seed(0)
 data=np.random.normal(loc=0,scale=1,size=100)
 data

```py
 fig,ax=plt.subplots()
 ax.boxplot(data)
 ax.set_xlabel('Data')
 ax.set_ylabel('Values')
 ax.set_title('Box Plot')
```
![image](https://github.com/user-attachments/assets/36d57c90-7ab5-4ee0-a2f3-ecce4b68f3ad)

```py
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```
![image](https://github.com/user-attachments/assets/18a66a2e-17db-46c7-a1a5-7caafe43205b)

```py
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
```


# Result:
Thus, the Data Visualization using matplot python library has successfully executed.
