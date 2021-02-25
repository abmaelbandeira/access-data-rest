# Accessing JPA Data with REST

Creating an application that accesses JPA relational data through a hypermedia-based RESTful front-end


## Dependencies
* JPA
* H2
* Rest Repository

## 1. Criar registro
`$ curl -i -H "Content-Type:application/json" -d '{"firstName": "Frodo", "lastName": "Baggins"}' http://localhost:8080/people`


## 2. Substituir dados
`$ curl -X PUT -H "Content-Type:application/json" -d '{"firstName": "Bilbo", "lastName": "Baggins"}' http://localhost:8080/people/1`


## 3. Atualizar
`$ curl -X PATCH -H "Content-Type:application/json" -d '{"firstName": "Bilbo Jr."}' http://localhost:8080/people/1`


## 4. Excluir registro
`$ curl -X DELETE http://localhost:8080/people/1`