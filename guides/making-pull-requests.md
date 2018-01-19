# Making a Good Pull Request

Goal: be as easy (for the maintainer) to merge as possible. (This means it can get merged faster.)

## Explain what you are trying to do

All pull requests should have a description explaining what their goal is. Stating a goal helps the maintainer evaluate whether the proposed change is the simplest way to achieve that goal. If the PR is just code then it is much harder to figure out the original intention of that code.

## Document what sort of change it is (patch, feature, breaking change)

What type of change you are proposing affects what you need to communicate.

The main types of changes are:
1. Patches
2. Features
3. Breaking changes

## Patches 
Bug fixing. Documenting this is easy. Explain the problem you intend to fix, and ideally also add a test case that reproduces the problem you found.

## Features
Adding new features is more challenging. Now your PR needs to explain the use-case. Consider the following when writing your PR:
- Why do you want this feature? 
- What problem are you trying to solve with it? 

When you make a pull request you are not just making a change to the code, you are also making a request to the maintainer: you are asking that they acknowledge this change and give this use their blessing. 

When possible, new modules are better than a PR, and then you can ask the maintainer to link to your module's README from their README.

Code style is considered but not usually a deal breaker for a PR, since code style change always change later. However, the API style is very important because breaking changes require changes throughout dependent modules.

For some really popular modules that a lot of code depends on, new features will require a very significant justification of why they are needed.

## Breaking Changes
Breaking changes are rare. However, if you must make a breaking change, one that restricts the API to a more minmal set is most likely to get merged. Expect a proposed breaking change to get lots of discussion.