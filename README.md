# Lunch-n-Learn

Talks, articles, papers that I watch or read during lunch time

### Talks

* [The insufficiency of good design by Sarah Mei](https://www.youtube.com/watch?v=UgrVdHYEZGg)
  * [Conway's Law](https://en.wikipedia.org/wiki/Conway's_law)
  * Good communication produces good code
  * Decoding smelly code
    * Hidden silos
    * Every piece of bad code is trying to say something
  * [Pair Programming](https://en.wikipedia.org/wiki/Pair_programming)
  * Create opportunities for informal communication

* [SOLID Object Oriented Design by Sandi Metz](https://www.youtube.com/watch?v=v-2yFMzxqwU)
  * [SOLID](https://en.wikipedia.org/wiki/SOLID_(object-oriented_design))
  * Rigid - Every change causes a cascade of changes
  * Fragile - Distant and unrelated changes with every other change
  * Immobile - You can't reuse anything
  * [Design Stamina Hypothesis](https://www.martinfowler.com/bliki/DesignStaminaHypothesis.html)
  * Only mock classes that you own
  * Don't mock/stub the object under test
  * The fact that there's a need to refactor doesn't mean you should
  * Don't be attached to your first idea
    * Embrace the code friction
    * If testing seems hard there's a problem with the design
    * TDD will punish you if you don't understand about design
  * [TDD Rules](http://agileinaflash.blogspot.com/2009/03/unclebobs-three-rules-of-tdd.html)
    * Refactor
      * Is the code [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself)?
      * Does it have one responsibility?
      * Does everything change at the same rate?
      * Does it depends that change less often than the unit itself?
  * Code Smells
    * Describing something using "and" implies that it does two different
      things
    * Describing something using "or" implies that it does two different and
      unrelated things
    * As soon as you feel resistant with arguments order that's a [data clump](https://en.wikipedia.org/wiki/Data_Clump_(Code_Smell))
      use a hash or value object
  * When testing - if it's going to change on production inject if not stub
  * Refactor not because you know which is the abstraction but because you want
    to find it.
  * [class_eval](https://www.jimmycuadra.com/posts/metaprogramming-ruby-class-eval-and-instance-eval)
  * It is better to depend on things that doesn't change often
  * TDD is not enough
  * DRY is not enough
  * Design because you expect your application to succeed

* [Less - The path to better design by Sandi Metz](https://vimeo.com/26330100)
  * What is design?
    * Not something establish by an architect but something you evolve through
      several iterations
  * Code needs to - work today, be able to change forever
  * Design purpose
    * Reduce the cost of change
  * [Design description](https://content.pivotal.io/blog/solid-object-oriented-design-sandi-metz)
    * Easily composable
    * Highly cohesive
    * Loosely coupled
    * Context independent
  * TRUE
    * Transparent - Consequence of change should be obvious
    * Reasonable - Cost of adding a new feature is proportional to it's value
    * Usable - If you write the code; you should be able to use it
    * Exemplary - More code like this should be good for your application
  * Knowledge is coupling
    * Create dependencies
    * Unstable dependencies increases risk
    * Try to always loose coupling
    * Uncertainty should be your guide

* [Therapeutic Refactoring by Katrina Owens](https://www.youtube.com/watch?v=J4dlF0kcThQ)
  * Guilt driven development
    * [Refactoring](https://martinfowler.com/books/refactoring.html)
  * [Characterization tests](https://en.wikipedia.org/wiki/Characterization_test)
    * Add test cases to discover what the code do right now
  * [Replace method with method object](https://sourcemaking.com/refactoring/replace-method-with-method-object)
    * To isolate the behavior
    * Rename methods in terms of what the method does
    * Follow longest lines to do extraction for clarification
      * Helps you identify a piece of code that does something and give it
        a name
  * [Code smells](https://sourcemaking.com/refactoring/smells)
  * Code junks
    * Comments
      * Do not echo the implementation
      * Do not be wrong or mispell
    * White spaces
    * Remove dead code
    * Needles parenthesis
    * Explicit default parameters
    * Unneeded dependencies
    * Too much hard work - simplify the code at every change
    * Duplicated tests
    * Combine all of the above


