# Dynamic_List_python
import pandas as pd

name1=[]
age1=[]

while True:
    
    name=input("what is your name ?")
    age=int(input("What is your age ?"))

    name1.append(name)
    age1.append(age)

    df=pd.DataFrame({'name':name1,'age':age1})
    print(df)

    df.to_csv('dynamic.csv')
    print('data inserted succesfully')

    x=int(input("1->do you want insert more data ?\n 2->exit ?"))
    if x==2:
        print("thanks")
        break
