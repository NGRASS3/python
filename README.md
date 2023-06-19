<img src="https://i.imgur.com/MSijigc.png" alt="Python"/>


<h1>Automating Security Tasks with Python</h1>
An important part of cybersecurity is controlling access to restricted content. In this turotial we'll develop an algorithm that parses a file containing IP addresses that are allowed to access restricted content and remove addresses that no longer have access.

<h2>Technologies Used</h2>

- Python

<p>
To start we will create 2 variables:

  1. import_file - which will hold our allow_list.txt (the file containing all the IP Addresses that are allowed access.
  2. remove_list - which is a list of all the IP Addresses no longer allowed access.
</p>

<img src="https://i.imgur.com/l2RhjRU.png" />

<p>
</br>
We start by opening the text file using the "import_file" variable, the "with" keyword, and the "open()" function with the "r" parameter. Running the "print(ip_addresses)" command at the bottom confirms our list of ip addresses is now copied as a string into the new variable "ip_addresses".
</p>

<img src="https://i.imgur.com/FnubF5a.png" />

<p>
</br>
After reading the file, we can now reassign the "ip_addresses" variable so its data type is updated from a string to a list. We use the ".split()" function to achieve this. Running "print(ip_addresses) confirms the change took place.
</p>

<img src="https://i.imgur.com/RKRqxki.png" />

<p>
</br>
Now we'll write code that removes elements of our "remove_list" variable from the "ip_addresses" list. We need an iterative statement to do this. We name the loop variable "element", loop through the "remove_list" and display each element. 
</p>

<img src="https://i.imgur.com/GysopZC.png" />

<p>
</br>
Now, in the body of the iterative statement we apply the ".remove()" method to the "ip_addresses" list and remove the ip addresses identified in the loop "element".
</p>

<img src="https://i.imgur.com/eGXyMrd.png" />

<p>
</br>
The final step will be to update the original file that was used to create "ip_addresses". We use the ".join()" method so the file can be updated. After the line with the ".join()" method, we build the "with" statement that rewrites the original file. Instead of "r" now we use "w" when calling the "open()" function to delete the contents in the original file and replace it with our new info. In the following screenshot I've documented what each piece of code does to sum up the turotial.</p>

<img src="https://i.imgur.com/8qPdgqT.png" />
