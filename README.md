# The Star Wars Galactic Map Project
The Star Wars Galactic Map Project is a crowd-sourced effort to maintain a thourough, comprehensive list of every planet in the Star Wars universe.

## Contributing
Please feel free to submit a PR or an issue adding or suggesting a planet for addition, editing, or removal.

## Schema
Each planet contains several fields:

* `Name` (string): The name of the planet.
* `Image` (string/null): The filename of the planet's image on Wookieepedia.
* `Coord` (string): The human-readable representation of the planet's coarse coordinate component.
* `X` (float): The machine-readable `x` coordinate of the planet.
* `Y` (float): The machine-readable `y` coordinate of the planet.
* `SubGridCoord` (string): The human-readable representation of the planet's fine coordinate component.
* `SubGridX` (float): The machine-readable `x` fine compoment coordinate of the planet, where `X+SubGridX` is the Planet's X coordinate.
* `SubGridY` (float): The machine-readable `y` fine compoment coordinate of the planet, where `Y+SubGridY` is the Planet's Y coordinate.
* `SunName` (string/null): The name of the planet's sun, or `null` if the planet a) doesn't have a sun or b) the information is unavailable.
* `Region` (string): The region of the planet.
* `Sector` (string): The sector of the planet.
* `Suns` (int): The number of suns the planet has.
* `Moons` (int): The number of moons the planet has.
* `Position` (int): The zero-indexed orbital position of the planet, or 0 (assumes interior orbit) if the information is unavailable.
* `Distance` (float): The distance from the Core in light years, or 0 if the information is unavailable.
* `LengthDay` (float): The length of one day on the planet in Standard Hours, or 24 (assumes standard day length) if the information is unavailable. 
* `LengthYear` (float): The length of one year on the planet in Standard Days, or 365 (assumes standard year length) if the information is unavailable. 
* `Diameter` (float): The diameter of the planet in kilometers, or 0 if the information is unavailable. 
* `Gravity` (float): The gravity of the planet relative to Standard Gravity, or 1 (assumes standard gravity) if the information is unavailable. 
