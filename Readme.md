Lets Learn Fetch API In Detail
With the help of fetch we can do CRUD opreation

fetch();
fetch(file/URL);-----> Promise
fetch(file/URL).then();
fetch(file/URL).then(function(response){
return response.data;// data depends like if its text then instead of data we will print text() or if it is in json then we will print json()
});
fetch(file/URL).then(function(response){
return response.data;
}).then(function(result){
console.log(result);
}).catch(function(error){
console.log(error);
});

// Now till now we,ve learned how to fetch the data from an API lets see now hwo to insert data in and API
the syntex looks like
fetch(file/URL,{
method:"POST", "PUT","DELETE",
body:data, it can be form data/JON Data/Text
header:{
    'content type' : 'application/json'
},

});
