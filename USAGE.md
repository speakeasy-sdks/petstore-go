<!-- Start SDK Example Usage [usage] -->
```go
package main

import (
	test "Test/v2"
	"context"
	"log"
	"net/http"
)

func main() {
	s := test.New()

	ctx := context.Background()
	res, err := s.Pets.CreatePets(ctx)
	if err != nil {
		log.Fatal(err)
	}

	if res.StatusCode == http.StatusOK {
		// handle response
	}
}

```
<!-- End SDK Example Usage [usage] -->