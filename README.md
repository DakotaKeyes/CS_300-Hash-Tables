# CS_300-Hash-Tables
Hash Tables 
Requirements & Rubric

The focus of these problems will be working with information extracted from a municipal government data feed containing bids submitted for auction of property. All materials for this lab assignment can be found in the Supporting Materials section below. The data set is provided in two comma-separated files:

eBid_Monthly_Sales.csv (larger set of 12,023 bids)
eBid_Monthly_Sales_Dec_2016.csv (smaller set of 76 bids)
This assignment is designed to explore linked lists, so you will implement a singly linked list to hold a collection of bids loaded from a CSV file. We provide a starter console program that uses a menu to enable testing of the hash table logic you will complete. It also allows you to pass in the path to the bids CSV file to be loaded, enabling you to try both files. In this version, the following menu is presented when the program is run:

***Menu:

Load Bids
Display All Bids
Find Bid
Remove Bid
Exit
Enter choice:***

The HashTable.cpp program is partially completed. It contains empty methods representing the programming interface used to interact with a hash table. You will need to add logic to the methods to implement the necessary behavior. Here is the public API for HashTable.cpp that you have to complete:

public:

HashTable();
virtual ~HashTable();
void Insert(Bid bid);
void PrintAll();
void Remove(string bidId);
Bid Search(string bidId);

Prompt
You will need to perform the following steps to complete this activity:

Setup: Begin by creating a new C++ project with a project type of "Hello World C++ Project".

Name the project “HashTable”. Remember to pick the correct compiler in Toolchains and click Finish. This will create a simple HashTable.cpp source file under the /src directory.
Download the starter program files and copy them to the project’s /src directory, replacing the existing auto-generated ones. Remember to right-click on the project in the Project Explorer pane on the left and Refresh the project so it adds all the new files to the src folder underneath.
Because this activity uses C++ 11 features, you may need to add the -std=c++11 compiler switch to the miscellaneous settings.

***Task 1: Define structures to hold bids. Hint: You may choose either an array or a vector for storage. Note that you may be able to reuse portions of your code from previous assignments to save you time. Look for places you have implemented vectors for storage or a Node structure for a linked list. Reusing code from these labs may save you time.

Task 2: Initialize the structures used to hold bids.

Task 3: Implement code to free storage when a class is destroyed.

Task 4: Implement code to calculate a hash value using the bid ID as the source for calculating the key.

Task 5: Implement code to insert a bid. Be sure to check for key collisions and use the chaining technique with a linked list to store the additional bids.

Task 6: Implement code to print all bids.

Task 7: Implement code to remove a bid.

Task 8: Implement code to search for and return a bid.***
