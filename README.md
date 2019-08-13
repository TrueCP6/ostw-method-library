# ostw-method-library
A method library for [Overwatch Script To Workshop](https://github.com/ItsDeltin/Overwatch-Script-To-Workshop/) by [Deltin](https://github.com/ItsDeltin/) to shorten code and generally make things easier. Post any suggestions, enhancements, or bugs in the issues tab.

## Method List
- `IsAIAccurate(player)` Whether the player is an AI or not. Works in more situations but it is more intrusive. by Deltin
- `IsAIUnintrusive(player)` Whether the player is an AI or not. Works in less situations but much less intrusive. by aLazyLion
- `OptimisedSphereHitbox(player, spherePosition, sphereRadius)` Whether the player is looking directly at the sphere. Has collision.
- `OptimisedEyeCastPosition(player, range)` Simplified RayCastHitPosition that casts a ray in the direction the player is looking.
- `SumOfArray(arrayToSum)`
- `AverageOfArray(arrayToAverage)`
- `OptimisedHorizontalDistance(point1, point2)` Returns distance as if both points were on the same y level.
- `OptimisedLinearInterpolate(point1, point2, fraction)` 1/2 as the fraction will give the midpoint between the points and 1/10 will return the point one tenth of the way along a straight line drawn between them. Fraction should be fraction of distance along straight line between points and must be less than 1 and greater than 0.
- `OptimisedLinearInterpolateDistance(point1, point2, distance)` Same as LinearInterpolate, but instead of going a fraction of the distance between points it goes a distance between points.
- `OptimisedTallnessOfPlayer(player)` Height of player measured from eyes to feet.
- `OptimisedIsOnScreen(player, point, fovOfPlayer)` Checks if a point is visible on screen to the player. 
- `SetHealth(player, health)` Sets the health of the player.
- `TallnessOfHero(hero)` Same as tallness of player, but instead gets the value for a hero.
- `NearestSolidSurface(point, accuracy)` Imperfect way of getting position of nearest solid surface. Accuracy is amount of times looped.
- `OptimisedSortedMedian(sortedArray)` Get median of array that is pre-sorted.
- `OptimisedUnsortedMedian(unsortedArray)` Get median of unsorted array.
- `OptimisedRange(inputArray)`
- `GenerateForeachArray(length)` Generates an array of a length where each value is equal to its index. Great for using for Filtered and Sorted arrays.
- `OptimisedBlendedIndex(array, index)` Allows you to get the index of an array as a non-integer. Blends the index lower and the index higher together in a weighted way. Array must be of multiplicable values (not player or string).

## Downloads
- [Releases](https://github.com/TrueCP6/ostw-method-library/releases/)
- [OSTW Releases](https://github.com/ItsDeltin/Overwatch-Script-To-Workshop/releases/)

## Installation
Installation instructions can be found [here](https://github.com/ItsDeltin/Overwatch-Script-To-Workshop/) for OSTW. Copy the contents of library.ostw into your project file.

## Usage
Once installed you can use the methods like you would any other action. NOTE: As of right now no methods can be used within the conditions tab. However you can work around this by using AbortIf(Not(condition)) at the beginning of the actions for each condition that uses a method (this has some limitations).