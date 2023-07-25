[githup](https://ahmadlotfyfalah1998.github.io/reading-notes/)
## Q1.What are the key components and purpose of Django Rest Framework (DRF) permissions, and how do they help in securing an API?
1.Serializers are used to convert Django QuerySets and model instances to (serialization) and from (deserialization) JSON <br>
(and a number of other data rendering formats like XML and YAML).<br>
2.Views (along with ViewSets), which are similar to traditional Django views, handle RESTful HTTP requests and responses.<br>
The view itself uses serializers to validate incoming payloads and contains the necessary logic to return the response. Viewsets are coupled with routers, <br>
which map the views back to the exposed URLs.<br>
## Q2.In SQL, what is the purpose of the SELECT statement, and how would you use it to retrieve all columns from a table called ‘employees’?
The SQL SELECT statement is used to retrieve records from one or more tables in your SQL database. The records retrieved are known as a result set.<br>
```
SELECT expressions
FROM tables
[WHERE conditions]
[ORDER BY expression [ ASC | DESC ]];
```
## Q3.Can you explain the role of DRF Generic Views and provide examples of their usage in building a RESTful API?

Code Reusability<br>
Simplified CRUD Operations<br>
Consistency<br>
Default Behavior<br>
Flexibility<br>
### examples
ListAPIView<br>
CreateAPIView<br>
RetrieveAPIView<br>
UpdateAPIView<br>
DestroyAPIView<br>
