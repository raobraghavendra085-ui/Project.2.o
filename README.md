# Project.2.o
#  Online Education Login Analysis (Python & Matplotlib)

This project demonstrates basic data visualization using **Python** and **Matplotlib** to analyze login patterns for an online education platform.  
The visualizations show how users access the platform across different devices and how mobile logins change over the week.
##  Features
 **Pie Chart** – Distribution of logins by device type  
 **Bar Chart** – Comparison of login counts across devices  
**Line Chart** – Mobile login trend over weekdays  
## Technologies Used

- Python 3.x  
- Matplotlib
   
##  Project Structure
## Visualizations Explained

##Login Distribution by Device (Pie Chart)

Shows the percentage of users logging in from:
- Mobile
- Laptop
- Desktop
- Tablet

##Login Count by Device (Bar Chart)

Compares the **number of logins** for each device type to identify the most commonly used platform.
## Mobile Login Trend (Line Chart)
Displays how mobile logins vary from **Monday to Friday**, helping identify usage patterns over the week.
##  Sample Data Used

devices = ['Mobile', 'Laptop', 'Desktop','Tablet']
logins = [550, 300，100，50]

## Pie Chart-Device usage Distribution

import matplotlib.pyplot as plt
devices = ['Mobile', 'Laptop', 'Desktop', 'Tablet']
logins = [550,300，100，50]
plt.figure()
plt.pie(logins, labels=devices, autopct='%1.1f%%',
startangle=90)
plt.title('Online Education Login Device
Distribution')
plt.show()

## Bar Chart-Device Login Comparison

import matplotlib.pyplot as plt
devices =['Mobile', 'Laptop', 'Desktop','Tablet']
logins = [550,300，100， 50]
plt.figure()
plt.bar(devices, logins)
plt.xlabel('Devices')
plt.ylabel('Number of Logins')
plt.title('Login Count by Device')
plt.show()

## Extension:Device Preference Trent 

days = ['Mon', 'Tue', 'Wed', 'Thu', 'Fri']mobile_logins =[100，120，130，110，140]plt.figure()
plt.plot(days, mobile_logins, marker='o')
plt.xlabel('Days')
plt.ylabel('Mobile Logins')
plt, title('Mobile Login Trend')
plt.show()
