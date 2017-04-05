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

* [Get a whiff of this by Sandi Metz](https://www.youtube.com/watch?v=PJjHfa5yxlU)
  * [Code smells](https://sourcemaking.com/refactoring/smells)
    * Bloaters
      * [Long method](https://sourcemaking.com/refactoring/smells/long-method)
      * [Large class](https://sourcemaking.com/refactoring/smells/large-class)
      * [Data clumps](https://sourcemaking.com/refactoring/smells/data-clumps)
      * [Long parameter list](https://sourcemaking.com/refactoring/smells/long-parameter-list)
      * [Primitive obsession](https://sourcemaking.com/refactoring/smells/primitive-obsession)
    * Tool abusers
      * [Switch statements](https://sourcemaking.com/refactoring/smells/switch-statements)
      * [Refused bequest](https://sourcemaking.com/refactoring/smells/refused-bequest)
      * [Alternative Classes w/ different interfaces](https://sourcemaking.com/refactoring/smells/alternative-classes-with-different-interfaces)
      * [Temporary field](https://sourcemaking.com/refactoring/smells/temporary-field)
    * Change preventers
      * [Divergent change](https://sourcemaking.com/refactoring/smells/divergent-change)
      * [Shotgun surgery](https://sourcemaking.com/refactoring/smells/shotgun-surgery)
      * [Parallel inheritance hierarchies](https://sourcemaking.com/refactoring/smells/parallel-inheritance-hierarchies)
    * Dispensables
      * [Lazy class](https://sourcemaking.com/refactoring/smells/lazy-class)
      * [Speculative generality](https://sourcemaking.com/refactoring/smells/speculative-generality)
      * [Data class](https://sourcemaking.com/refactoring/smells/data-class)
      * [Duplicated code](https://sourcemaking.com/refactoring/smells/duplicate-code)
    * Couplers
      * [Feature envy](https://sourcemaking.com/refactoring/smells/feature-envy)
      * [Inappropriate intimacy](https://sourcemaking.com/refactoring/smells/inappropriate-intimacy)
      * [Message chains](https://sourcemaking.com/refactoring/smells/message-chains)
      * [Middle man](https://sourcemaking.com/refactoring/smells/middle-man)
  * Every code smell has a refactoring recipe

* [Rampant Emergence: Lessons Learned from 4 Years of Aggressive Change by Neal Ford](https://vimeo.com/75256535)
  * Emergent design
    * Finding abstractions and patterns
    * Last responsible moment - It is safe to defer decisions?
      * Longer delay; more real data for decision
    * [Who needs an architect](https://martinfowler.com/ieeeSoftware/whoNeedsArchitect.pdf)
    * Architecture
      * Dynamic - Hard to change later
      * Static - web frameworks, tools. Allow few changes as possible
      * Product - features
      * Technical - Static/Dynamic
    * Traditional architect role
      * Define long term architecture up front
    * Agile architecture role
      * Few architecture elements and make them as flexible as possible
    * Don't do stupid things
      * Staff projects inadequately
      * Ramp up staffing too quickly
      * Assume good initial velocity on brand new X
      * Indulge in RDD (Resume Driven Development) - Put every single
        technology on your codebase
      * Anything on [Anti Patterns Catalog](http://c2.com/cgi/wiiki?AntiPatternsCatalog)
    * Be careful of architectural smearing
      * Produce afferent/efferent coupling between components
    * Stay in sync with upgrades
      * Tools, OS, frameworks
      * Future ported features are hard to refactor
      * Lingering upgrades == technical debt * 2
      * Age of codebase by number of components ongoing effort required for
        stasis
      * Especially true for "smeary" frameworks - Rails does this
      * Budget early as technical stories/tasks
    * Keep domain logic DRY
      * Business rules
      * Validations
      * Data rules
      * Workflow
    * Functionality must exist across tiers
    * Green to brown - when a project has some time in development
      * Every project hits an inflection point
      * Engineering practices should reflect the change
      * Add semi-permanent technical debts cards (Why not do refactoring every
        time someone touches the code?)
      * Harvesting model for reuse
      * Switch to emergent design styles
    * No design
      * No matter how much you try, requirements evolve chaotically
      * Bed-rock assumptions become malleable
    * Prefer dynamic over static
      * Don't think of the application as an equation
      * Make rules and policies dynamic
    * Loose coupling at integrations points
      * Early integration efforts focused on RPC-style interaction
      * Great for an equation bu lousy for a process
      * Resources over remote procedure calls
      * Choreography over orchestration
    * Coarse-grained components/services
      * Continuous delivery
    * Semantic monitoring
    * [Consumer driven contracts](http://martinfowler.com/articles/consumerDrivenContracts.html)
    * For brown field projects
      * Refactoring and restructuring exercises require increasing effort for
        the same result
      * Plan escalating effort towards remedial architecture and design
      * Trade off for reduced up-front effort

