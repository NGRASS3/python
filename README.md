<img src="https://i.imgur.com/MSijigc.png" alt="Python"/>


<h1>Automating Security Tasks with Python</h1>
An important part of cybersecurity is controlling access to restricted content. In this turotial we'll develop an algorithm that parses a file containing IP addresses that are allowed to access restricted content and remove addresses that no longer have access.

<h2>Technologie Used</h2>

- Python

<p>
To start we will create 2 variables:

  1. import_file - which will hold our allow_list.txt (the file containing all the IP Addresses that are allowed access.
  2. remove_list - which is a list of all the IP Addresses no longer allowed access.
</p>

<img src="https://i.imgur.com/l2RhjRU.png" />

<p>
</br>
We start by openening the text file useing the "import_file" variable, the "with" keyword, and the "open()" function with the "r" parameter. 
</p>

<img src="https://i.imgur.com/FnubF5a.png" />

<p>
</br>
After reading the file, we can now reassign the "ip_addresses" variable so its data type is updated from a string to a list. We use the ".split()" function to achieve this. Running "print(ip_addresses) confirms the change took place.
</p>

<img src="https://i.imgur.com/FnubF5a.png" />
