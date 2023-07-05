## C++ & mysql , a manage system for student and workers. 

### 1.Run stu.sql and workers.sql in terminal to create two tables `stu` and `workers`


### 2.For testing connection -->first way to solve it:

```linux
$ g++ test_connection1.cpp -o demo `mysql_config --cflags --libs`
```

### 3.For testing connection -->second way to solve it:

```linux
$ g++ test_connection2.cpp -o demo `mysql_config --cflags --libs`
```


### 4.CRUD for table `workers` 
```linux
## compile
ledger@ledger-Inspiron-5580:~/Desktop/E/mysql_connector_c++$ make
g++    -c -o worker_main.o worker_main.cpp
g++ -c worker_ms.cpp `mysql_config --cflags --libs`
g++ worker_main.o worker_ms.o -o worker_ms_demo `mysql_config --cflags --libs`
```

```linux
## run
ledger@ledger-Inspiron-5580:~/Desktop/E/mysql_connector_c++$./worker_ms_demo 
```


### 5.[Referrence](https://github.com/webary/MySQL_Tools)
