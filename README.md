# ostw-method-library
A method library for [Overwatch Script To Workshop](https://github.com/ItsDeltin/Overwatch-Script-To-Workshop/) by [Deltin](https://github.com/ItsDeltin/) to shorten code and generally make things easier. Post any suggestions, enhancements, or bugs in the issues tab.

## Method List
- `IsAI(player)` Whether the player is an AI or not. by Deltin
- `Pi()` Returns 3.146
- `SphereHitbox(player, spherePosition, sphereRadius)` Whether the player is looking directly at the sphere. Has collision.
- `EyeCastPosition(player, range)` Simplified RayCastHitPosition that casts a ray in the direction the player is looking.
- `Midpoint(point1, point2)` Midpoint between 2 vectors.
- `SumOfArray(arrayToSum)`
- `AverageOfArray(arrayToAverage)`
- `FOVTakenUpBySphere(distanceToSphereCenter, sphereRadius)` Angle of field of view a certain sphere will take up at a distance. When calculating distance using a player use Eye Position.
- `HorizontalDistance(point1, point2)` Returns distance as if both points were on the same y level.
- `LinearInterpolate(point1, point2, fraction)` 1/2 as the fraction will give the midpoint between the points and 1/10 will return the point one tenth of the way along a straight line drawn between them. Fraction should be fraction of distance along straight line between points and must be less than 1 and greater than 0.
- `LinearInterpolateDistance(point1, point2, distance)` Same as LinearInterpolate, but instead of going a fraction of the distance between points it goes a distance between points.
- `Pythag(side1, side2)` Returns length of hypotenuse.
- `Pythag(side1, hypotenuse)` Returns length of missing side.
- `ToKPH(metersPerSecond)`
- Imperial Units Conversion `ToMPH(metersPerSecond) ToFt(meters) ToYards(meters) ToInches(meters)`
- `TallnessOfPlayer(player)` Height of player measured from eyes to feet.
- `IsOnScreen(player, point, fovOfPlayer)` Checks if a point is visible on screen to the player. 
- `SetHealth(player, health)` Sets the health of the player.
- `GetMaxHealth(player)` Gets max health of player. If player is Tracer it will return 150.
- `PointFromPointDirectionDistance(startingPoint, direction, distance)` Returns point calculated from starting point going in a direction for a distance.
- `TallnessOfHero(hero)` Same as tallness of player, but instead gets the value for a hero.
- `NearestSolidSurface(point, accuracy)` Imperfect way of getting position of nearest solid surface. Accuracy is amount of times looped.
- `SortedMedian(sortedArray)` Get median of array that is pre-sorted.
- `UnsortedMedian(unsortedArray)` Get median of unsorted array.
- `MaxOfArray(inputArray)`
- `MinOfArray(inputArray)`
- `Range(inputArray)`

## Downloads
- [Releases](https://github.com/TrueCP6/ostw-method-library/releases/)
- [OSTW Releases](https://github.com/ItsDeltin/Overwatch-Script-To-Workshop/releases/)

## Installation
Installation instructions can be found [here](https://github.com/ItsDeltin/Overwatch-Script-To-Workshop/) for OSTW. Copy the contents of library.ostw into your project file.

## Usage
Once installed you can use the methods like you would any other action. NOTE: As of right now no methods can be used within the conditions tab. However you can work around this by using AbortIf(Not(condition)) at the beginning of the actions for each condition that uses a method (this has some limitations). Custom arrays seem to not work either as of now so try not to use them. Could just be me being dumb though ¯\_(ツ)_/¯.
