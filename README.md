---
<p align="center">
<img src="https://user-images.githubusercontent.com/72802400/147390953-1710cda5-3ec6-48bb-9e9a-545ed4f917ee.jpg" align="center"><img src="https://user-images.githubusercontent.com/72802400/147390801-6d7ec12e-b95a-4462-9816-05e6d87af24a.jpg" width ="90" height"100" align = "center">
</p>

---

# LRU-Cache-Implementation

### 1 - Scope
The purpose of this project is to implement a general purpose cache which using LRU replacement policy with the main goal to be as optimal as possible in terms of execution time of cache operations.

### 2 - Caching
Caches are auxiliary memories used to temporarily store data for future use. In general, a cache is used when a program / system searches for data from a data source (eg searching for files on a hard disk or database, information from the Internet. The program stores the information in the cache and the next time it searches for data from the data source, it first searches for it in the cache. If the data is in the cache (cache hit), the system saves time as it does not need to look at the data source to search for the data (it is much faster to get the data from the cache than from the source). In case the data is not in the cache (cache miss), the system retrieves the data from the source and stores it in the cache for future searches. In order to use a cache efficiently, the search time in the cache memory area must be much shorter than the time required to retrieve data from the data source.

<p align="center">
  <img src="https://user-images.githubusercontent.com/72802400/147883577-97d103ea-c37c-4c84-9aba-2516f49d1c50.png">
</p>

The memory space occupied by a cache is usually much smaller than the space occupied by the data source. When the cache space is filled with records, each time the process Store is called, the cache must delete a record in order to store the new data.The algorithm used to select the record to be deleted is called the Replacement Policy and plays a very important role in caching performance. The most common replacement policy is the Least Recently Used (LRU) policy. According to this policy, when the cache needs to delete a record, it deletes the record to which the last access is the least recent.

### 3 - Implementation

We used the following data structures to implement the LRU Cache.

i) Hashing with Separate Chaining<br/>
  We used Separate Chaining Hashing to achieve fast store and search times.
  
ii)Double Linked Lists<br/>
Double Linked Lists was used to implement Separate Chaining Hashing and for the implementation of the replacement policy Least
Recently Used.


![HashMap drawio ](https://user-images.githubusercontent.com/72802400/148103898-f028db9b-e188-43b0-9745-e0089dd1fde3.png)


### 4 - Check the stats

**Workstation Specifications**
- Windows 10 or Linux or MacOS, 64 bit
- RAM, 8GB required
- 128 GB Storage 
- 4 Core CPU

**Steps to run the cache and check the stats**
1. Clone this repository to Intellij
2. Run 'TestCacheSpeed' application from Intellij
3. Wait until cache serves all the requests
4. Check the stats to be printed in terminal

Note: If you want you can change the data file or the file with requests with the other files that provided with much more data to evaluate the system

### 5 - User Support
For help or new feature suggestions you can contanct with the development team.

