# getExternalIP
Get external IP from myexternalip.com.

Useful to get external IP of Google Cloud Engine or AWS instance wich gets inside (`eth` interfaces) only local network IP and get to outside world by NAT or Forwarding.

Using http://myexternalip.com web service.

Example usage:
```go
package main

import (
	"fmt"

	"github.com/geeksteam/getExternalIP"
)

// GetIP getting external IP from web service
func main() {
	fmt.Println("Your external IP is:'" + getExternalIP.GetIP() + "'")
}

```
