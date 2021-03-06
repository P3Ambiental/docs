# Java

Follow: https://google.github.io/styleguide/javaguide.html

Anything change will be added to this section

# Naming

* No shortened words anywhere unless otherwise specified - e.g. no btn, attr, ic, or anything else. Use full word all the time everywhere.

## File Naming

Follow: https://github.com/P3Ambiental/docs/blob/master/guides_and_standards/android_filenaming.md

# Best practices

Follow: https://developer.android.com/distribute/best-practices/

Any divergence shall be documented in this section. 

## Testing

Follow: https://developer.android.com/training/testing/

Any change will be docummented in this section.

### Tools: Unit Testing

* JUnit4
* ...

### Tools: UI Testing

TODO

## General Development Environment and Details

* Android Studio - Extremely recommended, but use anything else, such as Eclipse. Important that there are no conflicts or delays due to need of any tool that may conveniently be built into Android Studio. 
* Android API 15 and up
* Java 1.8
* Git

## Emulators and Device in Editor

### Phase 1: Target Pixel XL

* Emulator: Pixel XL, API 15, Android 4.03 (Google APIs)
* Device in Editor: Pixel XL, API 15

## Project Architecture

* [Clean Architecture](https://8thlight.com/blog/uncle-bob/2012/08/13/the-clean-architecture.html) - using Domain, Data, and Presentation layers.
* MVP - for Presentation layer. 

Resource: https://dev.to/wahibhaq/a-brief-summary-of-thoughts-on-clean-architecture-and-mvp-48h9

The android project will utilise the Clean Architecture and have a Domain, Data, and Presentation layers. Each of these layers be a distinctive module respectively. The Domain Layer will be a Java Library module. The Data Layer will be an Android Library module. The Presentation Layer will utilise the default `app` module created by Android Studio for new Projects. 

Further Resources:

* https://android.jlelse.eu/a-complete-idiots-guide-to-clean-architecture-2422f428946f
* https://proandroiddev.com/creating-clean-architecture-multi-project-mvp-app-34d753a187ad

## Anything Else

Always: https://developer.android.com

Any divergance will be documented. 

# Contributing

## Workflow

* Make your own development branch. Checkout from `development`. 
* Format your branch name as `dev_githubhandle`. Single underscore between `dev` and your github handle. Make sure the branch name is entirely lowercase.
* Do not make direct pull requests with `master`.
* Make frequent pull requests with `development`.


## Commit Message

https://chris.beams.io/posts/git-commit/


# Phases and Versioning

TODO
