# goapi
Voorbeeld rest api in golang van youtube kanaal Alex Mux

starten in cli vanuit doapi directory met:

```zsh
$ go run cmd/api/main.go

Starting GO API service...

 ______     ______        ______     ______   __    
/\  ___\   /\  __ \      /\  __ \   /\  == \ /\ \   
\ \ \__ \  \ \ \/\ \     \ \  __ \  \ \  _-/ \ \ \  
 \ \_____\  \ \_____\     \ \_\ \_\  \ \_\    \ \_\ 
  \/_____/   \/_____/      \/_/\/_/   \/_/     \/_/ 

$ curl -H "Authorization:789GHI" http://localhost:8000/account/coins/\?username=marie
{"Code":200,"Balance":300}

$ curl -H "Authorization:789ABC" http://localhost:8000/account/coins/\?username=marie
{"Code":400,"Message":"Invalid username or token."}

$ curl -H "Authorization:789GHI" http://localhost:8000/account/coins/\?username=peugeot404
{"Code":400,"Message":"Invalid username or token."}
```
