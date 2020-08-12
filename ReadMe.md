# dev.to API
### A consumed dev.to API using Go

* Still under construction but usable.

```go
package main

import(
	"fmt"
	"github.com/edwinnduti/devto-api"
)

func main(){
	//capture title and description from user nduti
	titles,descriptions,err := devto-api.GetTitles("nduti")

	//handle errors
	if err!=nil{
		fmt.Println(err)
	}

	//loop through to traverse them
	for n,_ := range titles{
		fmt.Println(titles[n],"\n",descriptions[n],"\n")
	}

}
```
* just alittle more 
