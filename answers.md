1. In Mocha, what are the differences between before after beforeEach afterEach? When do they run? What are they used for?
## They are called hooks, and are used to set up preconditions and will be cleaned up after the tests.
## before() and after() hooks only run once, beforeEach() and afterEach() hooks run every time before or after the tests.
## The order is like this: before(once) -> beforeEach() -> test -> afterEach(); beforeEach() -> test -> afterEach(); ... -> after(once)


2. What is the point of Test Driven Development? What do you personally think about this approach?
## Writing test codes before the real API, this is TDD. Anytime during the API development, developer can get a reliable and usable product with less bugs. The traditional tests are written after the production, and try to find as many bugs as possible, but TDD can make sure as less bugs as possible even before starting to develop the product. 
## TDD has more work to do, developer has to plan well before product, write testing code before all new features. For a newbie like myself, I don't think I have this kind of ability now to plan a project so well before i see the real thing.


3. What is a spy in sinon? How do we use it to effectively test a callback?
## Spy is a function that records arguments, return value, and throw errors for its calls. We can use spy to test if a function was called or not, how many time a funtion should be called.