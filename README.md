# snippetbox
This is a web application to save snippets, based on the book `let's go` by [alex edwards](https://www.alexedwards.net/).
This application uses `Golang` and it's powerful standard library to server a complete web applicaiton.

### Requirements
- Golang version 1.11 or higher
- Mysql (driver)[github.com/go-sql-driver/mysql]

### Libraries
- github.com/golangcollege/sessions v1.2.0
- github.com/justinas/alice v1.2.0
- github.com/justinas/nosurf v1.1.0

### Running
You can pull the code run it in developmnet mode:
```
  cd snippetbox
  go run cmd/web/!(*_test.go)              //to run without tests
  go test -v cmd/web/*   //to run the test
  
```
### Building
You can pull the code and create a binary file to run the application anywhere:
```
  cd snippetbox
  go build -o snippetbox cmd/web/*             //to run without tests
  
```
### To Do
-[] Creating an API endpoint which returns a JSON representation of a snippet
-[] Adding functionality to confirm a user’s email address on signup
-[] Adding functionality for a user to reset their password
-[] Creating a command line application under cmd/cli to carry out database admin tasks
