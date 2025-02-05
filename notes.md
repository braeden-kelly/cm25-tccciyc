- Concerns
  - Duplicative code
- Separation of concerns
  - Don't let plumbing code pollute your software
- Common factors or concerns
  - Validation
  - Error handling
  - Logging
  - Data access
  - Business logic
  - UI logic
  - Authorization
  - Caching 
- Can write/use linter to visualize concerns
- Cross cutting concerns
  - Concerns that apply across multiple individual use cases 
- Osi model
  - Confining things in layers
- Use result pattern for bad results and capture true exceptions in middleware
- Decorator 
  - Good
    - Separation of concerns
    - Single responsibility
    - Simpler real work
    - Flexible to implement
  - Bad
    - More classes (a lot more) 
    - More complexity
    - More work setting up DI
- Mediator
  - Library that allows you to decouple things
  - Event driven
  - Every handler has a common handle method
    - Makes decorating easy
- Chain of responsibility
  - Position units of logic in a callable sequence 
  - Each class or method performs some work then calls the next
  - Don't have to write lots of decorators, just one moddleware
  - Basically just interceptors
  - Likely going to require some reflection for certain behaviors like cache
    - Could be performance concern 
    - More complicated to not log sensitive properties
  - There's a attributed behaviors package that can be used instead of program configuration
- Can be mixed and matched with program configured behaviors
