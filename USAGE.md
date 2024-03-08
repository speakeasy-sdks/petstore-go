<!-- Start SDK Example Usage [usage] -->
```go
package main

import (
	test "Test/v3"
	"context"
	"log"
)

func main() {
	s := test.New()

	ctx := context.Background()
	res, err := s.Pets.CreatePets(ctx)
	if err != nil {
		log.Fatal(err)
	}
	if res != nil {
		// handle response
	}
}

```
<!-- End SDK Example Usage [usage] -->