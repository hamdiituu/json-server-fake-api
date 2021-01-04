intall steps 
<br/>

npm install -g json-server

server run command : 

json-server --watch data.json


crud methods : 

<br>
all data

method (get) : http://localhost:3000/movies

return : 
[
    {
        "title": "hamdd",
        "cover": "typicode",
        "id": 1
    },
    {
        "id": 2,
        "title": "json-server 2",
        "cover": "typicode"
    },
    {
        "title": "json-server",
        "cover": "typicode",
        "id": 3
    }
]

<br>

data with id 

<br>

method (get) : http://localhost:3000/movies/1

return :

{
    "title": "hamdd",
    "cover": "typicode",
    "id": 1
}


<br>

add data :

method (post) : http://localhost:3000/movies

request body : 
{
        "title": "hamditug",
        "cover": "typicode"
}

return :
{
        "title": "hamditug",
        "cover": "typicode"
}

<br>
update data :

mehtod (put) :  http://localhost:3000/movies/1

request body :
{
        "title": "test put",
        "cover": "typicode"
}
return : 
{
    "title": "hamdd",
    "cover": "typicode",
    "id": 1
}

<br>
delete data :

method (delete) :http://localhost:3000/movies/1

return : {}

<br>

query search  :

method (get) :http://localhost:3000/movies?title=json-server

return :

[
    {
        "title": "json-server",
        "cover": "typicode",
        "id": 3
    }
]