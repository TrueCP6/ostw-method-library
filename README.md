# ostw-method-library
A method library for [Overwatch Script To Workshop](https://github.com/ItsDeltin/Overwatch-Script-To-Workshop/) by [Deltin](https://github.com/ItsDeltin/) to shorten code and generally make things easier. Post any suggestions, enhancements, or bugs in the issues tab.

## Method List
- `SumOfArray(arrayToSum)`
- `AverageOfArray(arrayToAverage)`
- `TallnessOfHero(hero)` Same as tallness of player, but instead gets the value for a hero.
- `NearestSolidSurface(point, accuracy)` Imperfect way of getting position of nearest solid surface. Accuracy is amount of times looped.
- `GenerateForeachArray(length)` Generates an array of a length where each value is equal to its index. Great for using for Filtered and Sorted arrays.

## Downloads
- [Releases](https://github.com/TrueCP6/ostw-method-library/releases/)
- [OSTW Releases](https://github.com/ItsDeltin/Overwatch-Script-To-Workshop/releases/)

## Installation
Installation instructions can be found [here](https://github.com/ItsDeltin/Overwatch-Script-To-Workshop/) for OSTW.
Download the method library from [the releases page](https://github.com/TrueCP6/ostw-method-library/releases/) and copy it to the same folder as your OSTW project file.
At the top of your project file add `import "library.ostw";`.

## Usage
Once installed you can use the methods like you would any other action. NOTE: No methods in this library can be used within the conditions tab. However you can work around this by using AbortIf(Not(condition)) at the beginning of the actions for each condition that uses a method (this has some limitations).