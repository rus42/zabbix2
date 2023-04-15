Васёв А.В.
Система мониторинга Zabbix. Часть 2

Задание 1

![alt text](https://github.com/rus42/zabbix2/blob/main/Task_1.1.png)
![alt text](https://github.com/rus42/zabbix2/blob/main/Task_1.2.png)
![alt text](https://github.com/rus42/zabbix2/blob/main/Task_1.3.png)

Задание 2,3

![alt text](https://github.com/rus42/zabbix2/blob/main/Task_2_3.png)

Задание 4

![alt text](https://github.com/rus42/zabbix2/blob/main/Task_4.png)

Задание 5

![alt text](https://github.com/rus42/zabbix2/blob/main/Task_5.png)

Задание 6

![alt text](https://github.com/rus42/zabbix2/blob/main/Task_6.1.png)
![alt text](https://github.com/rus42/zabbix2/blob/main/Task_6.2.png)

import sys
import os
import re
import datetime
if (sys.argv[1] == '1'):
    	print(f"VasevAV")
elif (sys.argv[1] == '2'):
    	print (datetime.date.today())
else:
    	print(f"netology")

Задание 7

![alt text](https://github.com/rus42/zabbix2/blob/main/Task_7.1.png)
![alt text](https://github.com/rus42/zabbix2/blob/main/Task_7.2.png)

import sys
import os
import re
import datetime

if (sys.argv[1] == '-ping'):
    	result=os.popen("ping -c 1 " + sys.argv[2]).read()
    	result=re.findall(r"time=(.*) ms", result)
    	print(result[0])
elif (sys.argv[1] == '-simple_print'):
    	print(sys.argv[2])
elif (sys.argv[1] == '1'):
    	print(f"VasevAV")
elif (sys.argv[1] == '2'):
    	print (datetime.date.today())
else:
    	print(f"netology")


Задание 8

![alt text](https://github.com/rus42/zabbix2/blob/main/Task_8.1.png)
![alt text](https://github.com/rus42/zabbix2/blob/main/Task_8.2.png)
![alt text](https://github.com/rus42/zabbix2/blob/main/Task_8.3.png)
![alt text](https://github.com/rus42/zabbix2/blob/main/Task_8.4.png)







