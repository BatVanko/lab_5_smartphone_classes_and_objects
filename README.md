# lab_5_smartphone_classes_and_objects

Create a class called Smartphone. Upon initialization, it should receive a memory (number). It should also have 2 other instance attributes: apps (empty list by default) and is_on (False by default). Create 3 methods:
-	power() - sets is_on on True if the phone is off, otherwise sets it to False
-	install(app, app_memory)
o	If there is enough memory on the phone and it is on, installs the app (add it to apps and decrease the memory of the phone) and returns "Installing {app}"
o	If there is enough memory, but the phone is off, returns "Turn on your phone to install {app}"
o	Otherwise, returns "Not enough memory to install {app}"
-	status() - returns "Total apps: {total_apps_count}. Memory left: {memory_left}"

Test Code
smartphone = Smartphone(100)
print(smartphone.install("Facebook", 60))
smartphone.power()
print(smartphone.install("Facebook", 60))
print(smartphone.install("Messenger", 20))
print(smartphone.install("Instagram", 40))
print(smartphone.status())

Output
Turn on your phone to install Facebook
Installing Facebook
Installing Messenger
Not enough memory to install Instagram
Total apps: 2. Memory left: 20

