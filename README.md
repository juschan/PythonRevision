# Python Revision

## Python Dictionaries and JSON
Python dictionaries are used to store a set of key-value data.
```python
Employee = {'EMP001': 'Jane Smith', 'EMP002': 'Tom Jones', 'EMP003': 'Mary Tan'}
```
Python dictionary keys must be unique, and immutable (ie. of type string, numbers or tuples)


JSON (JavaScript Object Notation) is a file format consisting of key-value pairs and array data types.
JSON is almost identical to JavaScript objects. However,  
- For JSON, keys must be strings and written with double quotes. 
- For JavaScript, keys can be strings, numbers or identifier names.


### Notes
- Do not assume Python dictionaries and JSON are directly interchangeable.
- Use the Python package, json, to work with JSON data
```python
import json
...
```

## Web Protocol
Many protocols involving the web/internet, many of them are layered and depedent upon each other.

HTTP (Hyptertext Transfer Protocol) is a common web protocol. Common used when browsing the web.

[HTTP Basics](https://www.ntu.edu.sg/home/ehchua/programming/webprogramming/HTTP_Basics.html)



## MongoDB

Basic code to access MongoDB.

Does not work on corporate desktop: pymongo.errors.ServerSelectionTimeoutError.

```python
from pymongo import MongoClient
client = MongoClient('mongodb://MyUserName:password1234@ds245170.mlab.com:45170/pydotaia', connect=False)
db = client['pydotaia']
collection = db['cpu_mem']
cursor = collection.find({})
for doc in cursor:
    print(doc)
```


## Web Development
Web development mainly centred on HTML, CSS and JS.

- HTML - HyperText Markup Language (for structure and content)
- CSS - Cascading Style Sheets (for consistent styling and design)
- JS - Javascript programming language (for interactivity, functionality)

VS Code editor provides several conveniences when creating websites.
- Syntax highlighting for HTML, CSS and JS
- IntelliSense for javascript
- Emmet for shortcuts
