# airlines-integrations

Centralized interface for airlines integrations

## Testing
```bash
# All test
grails test-app

# Only unit
grails test-app :unit

# Only integration
grails test-app :integration

# Only functional
grails test-app :functional
```

## Debugging (tests)
Debugging is hard but not impossible. Basic guidelines:
* Run the tests as grails tests, not as JUnit. This is crucial
* The debugger can´t follow groovy´s dynamic dispatch in some cases. Place breakpoints on all derived implementations, if needed
* When switching between git branches, the tests will fail on the first run due to invalid class caches. Try again
* Don´t run console tests during debugging, since the console test runner will hang
