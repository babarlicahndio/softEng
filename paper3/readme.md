# Paper 3

## summary 3

### title:Using Other's tests to identify breaking updates.

Developers are using third party apps for software developent for adding new patches and features but there are alot of problems faced by developers some times the software cause break down or caught bugs.
Now a days software development are bieng complex and most of the softwres are not built from scratch but rather leverage others codeToday’s software systems are large and complex.

Many of these software systems are not built from scratch, but rather leverage others code that has been built in the past to accelerate their own  development. One particular driver of this code reuse is the growing  popularity of software ecosystems such as Node.js PackageManager (npm)  which provides a platform for developers to share their own and use others’ code.
Code reuse has m any advantages, including allowing software  systems to be developedfaster, include richer features, and even  achieve higher quality. However, this often comes at an increased cost of having to manage these dependencies. Specifically, as the software evolves (and its dependencies do as well), updating these dependencies can become more risky.
To ensure the stability and quality of newly released dependencies, developers often run their own tests. This has proven tobe a good solution and some tools  support the automation of such approaches. However, in many cases,  developers are still forced to“rollback” updates to packages because they introduce regression in their system functionality.

To detect breakage-inducing versions, we execute the tests of dependent projects that depend on the priorversion of the target dependency.For those tests that passon the priorversion,were execute them after updating the target dependency to the newer version.Tests that pass the execution on the prior version but not  the execution on the newer version may indicate that the newer  version has introduced a breakage.
The technique runs tests from dependent projects before and  after updating a target dependency from a prior version to a newer  version. Unless an update is intentionally breaking backwards compatibility (e.g., a major release), the tests from the prior version should continue to pass in the new version.



[Back](../readme.md)