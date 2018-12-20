1. 首先访问 localhost:8080/,正常返回信息；
2. 访问localhost:8080/users，提示没有权限；
3. 登陆 localhost:8080/login，带上json信息：
```{
	"username":"admin",
	"password":"password"
}```
，会返回头信息。
Authorization →Bearer eyJhbGciOiJIUzUxMiJ9.eyJzdWIiOiJhZG1pbiIsImV4cCI6MTU0NjE1MTg2OH0.3omoRhXaCqcX-kkjqW2ivZHl0dFuQ5FZWzphduqrL2u_uQPDMM0AXAPpzNKjXo3iZyanXKUjFil7EzTrigk5Tg
4.带上头信息：Authorization-> eyJhbGciOiJIUzUxMiJ9.eyJzdWIiOiJhZG1pbiIsImV4cCI6MTU0NjE1MTg2OH0.3omoRhXaCqcX-kkjqW2ivZHl0dFuQ5FZWzphduqrL2u_uQPDMM0AXAPpzNKjXo3iZyanXKUjFil7EzTrigk5Tg
访问localhost:8080/users，会返回user信息。
