# Reading Notes 01

## Responsive Web Design

Responsive web design describes the the practice of designing a website that is univerally functional. What this means is that a website needs to work properly regardless of the device it is being used on. This is more in relation to screen size and an operating system's browser, but it also related to different version of software or hardware,say, if someone is using a slightler outdated smartphone, computer, or other device. This term was initially coined by a man named Ethan Mercotte who wrote a book of the same title.

Responsive design encapsillates design that is quick-reacting (an underlying meaning of the word), design that is Adaptive or built with a few presets in mind, or design that is Mobile or deisgned especially for mobile viewing. Mobile sites are generally 'light' versions of the desktop site, but serve the same general purpose.

### Flexible Layouts

#### Flexible Grids

Flexible grid systems are measured in relative width units which allows for the grid format to work regardless of viewport width. The units can either jsut be percentages, or they can be em unites which should work just the same.

#### Media Queries

Media queries allow for the detection of the viewer's device and can change the overall format depending on what the query returns. This can change styles based on the device itself, the viewport width, the aspect ratio of the screen, or even the pixel ratio etc. The best way to link a stylesheet with this in mind is to use ```@media``` or ```@import```. This allows for further customization with logical operators to choose a style that is ideal for a certain circumstance. Another popular technique is to target mobile devices first, the expand the features as the device viewport gradually widens. This is referred to as 'Mobile First'.

#### Flexible Media

Some media is formatted in certain ways that makes it not scalable by default. To change this, the size media like videos or pictures takes up on the screen needs to be set manually. Using max-height and max-width properties is an easy solution. For more complex things like embedded media or iFrames, other measures need to be taken specific to each case.

## Floats

Float is the CSS property that allows items to be positioned to the left or right of an HTML element and have other inline content flow around it. This can be used on whole webpages, but it is inferior to other techniques. It's best use is for styling within smaller elements. It can take right, left, inherit, or none as values.

The sister property to ```float``` is ```clear``` which puts it on its own unique line in relation to other floats. It can take left, right, or none as values.

Of importance to note is that if an element only contains floating items, then its height will collapse to zero despite the flaoting objects themselves appearing to have their own heights. There are a few fixes to do this, but one popular method is to have an empty div with the property ```clear: both;``` to essentally act as a line break for the div with only floating elemnts inside of it.

Lastly, there are a slew of bugs that may pop up while using float. Because of this it is given the 'fragile' reputation. There are fixes for them, but they need to be researched on a case by case basis.

## CSS Grids

Here are a few trips to help with the use of grid systems:
- Keep it simple: Use simple names to keep track of which element is supposed to be how wide.
- use ```box-sizing: border-box``` to keep an element the same width regardless of changes to padding, border, or margin.
- Apply a fixed padding to the right of all columns except the last one.
- If you want gutters for the page, add padding to the left (top and bottom are optional), then reset the padding on the rightmost element



#### [Home](README.md)