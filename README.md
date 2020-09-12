# C# Framework Design

## Designing Framework:
### => A software framework in computer programming is an abstraction in which common code providing generic functionality can be selectively overridden or specialized by user code providing specific functionality.

### => A framework can be a library of code that performs a special task or a more complicated foundation in our codebase that handles complex systems, and even renders logic critical for our application to run.

### => .NET is a collection of APIs and services that help us speed up our own development.

## 1. When Writting Our Framework:
### => It's important to keep in mind that we'll want to create a goal and find the simplest solution to achieve it.

## 2. Designing Frameworks:
### => Requires a lot of planning and special architecture consideration.

## 3. What a Framework Represents:
### => A core pillar of a project's code, it needs to be bug free, easy to implement, and more important , scalable for future changes or additions to the codebase.

## 4. Portability (The Final Components):
### => The final component of any good framework is portability - whether we can isolate our framework and easily share it with others.

### => Good code architecture is not just about coding - it is about not trying to reinvent the wheel.

## Try to Answer the Following Things While Developing a Framework:
### => 1) Is there an existing library that does what we are trying to do?
### => 2) Can the framework stand on its own? If not, what does it depend on and will others be able to use it?
### => 3) How can we simplify the functionality of the framework to its core components and only include that in your code?

## What Sharing a Framework Requires:
### => 1. Clean API architecture
### => 2. Documentation
### => 3. Clear functionality

## Things to Keep in Mind During Development:
### => 1) Don't Boil the Ocean: Most software is made of several frameworks. It's OK to design several self-contained frameworks that work together as one larger whole, which is how .NET works.
### => 2) Limit Dependencies: When encapsulating frameworks by functionality, it helps to limit dependencies.
### => 3) Clearly State Dependencies: It's OK for framework to depend on other frameworks. Just be clear about what is needed to run the library for a developer looking to use it in their own code.

## Ways of Sharing Framework:
### => Creating Dynamic Link Library (.dll from Shared Project)
### => NuGet
### => Hosting Online (GitHub, BitBucket, GitLab, Own Website, etc.)

## Things to Look For During Publishing the FrameWork Code Online:
### => Track bugs.
### => See progress.
### => Allow contributions.

### => To Know More about Licenses: https://opensource.org/licenses/

## Encapsulations:
### => Encapsulation is used to hide the values or state of a structured data object inside a class, preventing unauthorized parties' direct access to them.
### => Encapsulation is a key concept in object-oriented programming, and it helps to not only protect the data inside of our framework but also simplify the external interaction with the undelying code.

## Ways to Encapsulate Data:
### => 1. Define strict scope for our framework APIs.
### => 2. Any externally facing code should be made public.
### => 3. Internal code should be made protected.
### => 4. Code that is designed to be extended or changed should be marked as virtual.
### => 5. And anything that is final should be marked as read-only, static, or sealed.

## Scope:
### => This scope starts at the class level. Any class can be made public, private or internal.

## Public APIs:
### => Take a look at the classes own APIs and see which should be exposed to the user, by making them public, and hide the rest through protected scope.

## Avoid Private Scope:
### => Avoid private scope when possible. While code can be hidden from the public methods, try to create protected methods that can still be extended and changed by using the protected virtual scope.

## Protecting Data:
### => Acoid directly manipulating data passed into methods. We don't want our framework to corrupt that data. Make a ccopy and manipulate that instead of the actual source.
### => If we can't make a copy of the data, use the ref argument to clearly state that properties passed into a method will directly manipulate the objects themselves.

## Interfaces:
### => Interfaces provide an opportunity to build a very modular framework and offer developers additional ways to extend and enhance what may be very closed system.

## Self asked Questions During Framework Developemnt:
### => 1. Does It Do What Others Need?
What happens when someone needs to do X, Y, or Z?

### => 2. Can It Scale?
Can our framework scale to the needs of the user or are we building a tool that is not flexible?

### => 3. Can It Be Extended?
Can users extend what we have done and build on the top of it easily.

## Tips for Building Modular Classes:
### => 1) Interfaces 
Does the class implement an interface?

### => 2) Support Extending:
Is the class sealed or do we expect developers to extend it?

### => 3) Abstract Classes:
Are we creating abstract classes and base classes as a layer of foundation, or is the class a concreate implementation with no inheritance?

### => 4) Utilities:
What kind of utilities classes do we provide? Are they singletons or can they be extended?

### => 5) Primitive Classes:
What are the primitive classes of our framework ? Are these enough? Can they be used outside of the framework, or are they closely ties to the intended use case?

### => 6) Sharing the Code:
Are we sharing the code for our framework and do we intend others to extend it beyond its original design, or would we rather keep it private?

## Extending Framwork:
### => 1) What are we solving?
What are the use cases the framework solves that others will use it for?

### => 2) Gaps?
What gaps are there in framework?

### => 3) Fixes?
How do we intend for the others to fix these gaps?

### => While designing a framework, it helps to use it ourself.















