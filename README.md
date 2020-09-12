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





