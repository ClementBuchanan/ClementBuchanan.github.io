# CSS Transforms, Transitions and Animation

## CSS Transforms
The transform CSS property lets you rotate, scale, skew, or translate an element. It modifies the coordinate space of the CSS visual formatting model. Only transformable elements can be transformed. That is, all elements whose layout is governed by the CSS box model. Here are some sample syntax for it:

- transform: perspective(17px);
- transform: rotate(0.5turn);
- transform: rotate3d(1, 2.0, 3.0, 10deg);
- transform: rotateX(10deg);
- transform: rotateY(10deg);
- transform: rotateZ(10deg);
- transform: translate(12px, 50%);
- transform: translate3d(12px, 50%, 3em);
- transform: translateX(2em);
- transform: translateY(3in);
- transform: translateZ(2px);
- transform: scale(2, 0.5);

CSS transform property have many types:

- ***2D Transforms*** - Elements may be distorted, or transformed, on a two-dimensional plane. It works on the x and y axes, known as horizontal and vertical axes. 
- ***Combining Transforms*** - It is common for multiple transforms to be used at once, rotating and scaling the size of an element at the same time for example.
- ***Transform Origin*** - The transform-origin property can accept one or two values. When only one value is specified, that value is used for both the horizontal and vertical axes. If two values are specified, the first is used for the horizontal axis and the second is used for the vertical axis.
- ***Perspective*** - In order for three-dimensional transforms to work the elements need a perspective from which to transform. The perspective for each element can be thought of as a vanishing point, similar to that which can be seen in three-dimensional drawings.
- ***3D Transforms*** - Using three-dimensional transforms we can change elements on the z axis, giving us control of depth as well as length and width. Here's a sample HTML and CSS code for this:
              
**CSS**
.original {
  perspective: 200px;
}
.box {
  transform: rotateX(45deg);
}
.original-1 {
  perspective-origin: 0 0;
}
.original-2 {
  perspective-origin: 75% 75%;
}
.original-3 {
  perspective-origin: 20px 40px;
}

- ***Transform Style*** - On occasion three-dimensional transforms will be applied on an element that is nested within a parent element which is also being transformed. In this event, the nested, transformed elements will not appear in their own three-dimensional space.
- ***Backface Visibility*** When working with three-dimensional transforms, elements will occasionally be transformed in a way that causes them to face away from the screen. This may be caused by setting the rotateY(180deg) value for example. Here's a sample HTML and CSS code for this:

**CSS**
.box-1 {
  transform: rotateY(180deg);
}
.box-2 {
  backface-visibility: hidden;
  transform: rotateY(180deg);
}

## CSS Transitions & Animations
CSS has rhe ability to write behavior for tansitions and animations withouth the use of Javascript or flash. With CSS3 transitions we now have the potential to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted. The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes. There are four properties:

1. Transition-property
1. Transition-duration
1. Transition-timing-function
1. Transition-delay

## 8 simple CSS3 transitions
There are umpteenth posibilities for UX designers using CSS and they only require a few lines of codes. Here a a few of them:

1. ***Fade-in*** - Fade in effects are coded in two steps: first, you set the initial state; next, you set the change, for example on hover.
1. ***Change color*** - Simplly set the div’s class to “color” and specify the color we want in our CSS.
1. ***Grow and shrink*** - To grow an element set your div’s class to “grow” and then add this code to your style block.
1. ***Rotate elements*** -  Give your div the class “rotate” and add the following to your CSS:

.rotate:hover
{
        -webkit-transform: rotateZ(-30deg);
        -ms-transform: rotateZ(-30deg);
        transform: rotateZ(-30deg);
}

1. ***Square to circle*** - Give your div the class “circle” and add this CSS to your styles:

.circle:hover {
  border-radius:50%
}

1. ***3D shadow*** - Give your div the class “threed” and then add the following code to your CSS:

.threed:hover
{
        box-shadow:
                1px 1px #53a7ea,
                2px 2px #53a7ea,
                3px 3px #53a7ea;
        -webkit-transform: translateX(-3px);
        transform: translateX(-3px);
}

1. ***Swing*** - Not all elements use the transition property. We can also create highly complex animations using @keyframes, animation and animation-iteration.

1. ***Inset border*** - Give your div the class “border” and add the following CSS to your styles:

.border:hover {
  box-shadow: inset 0 0 0 25px #53a7ea;
}

## Animated Buttons
Using the tranform properties of CSS animated button can also be created. 

## CSS3 Animations: Keyframes
CSS animations make it possible to animate transitions from one CSS style configuration to another. Animations consist of two components, a style describing the CSS animation and a set of keyframes that indicate the start and end states of the animation’s style, as well as possible intermediate waypoints. To create the animation sequence style the element you want to animate with these animation sub-properties:

* ***animation-name*** - Specifies the name of the @keyframes at-rule describing the animation’s keyframes.
* ***animation-duration*** - Configures the length of time that an animation should take to complete one cycle.
* ***animation-timing-function*** - Configures the timing of the animation; that is, how the animation transitions through keyframes, by establishing acceleration curves.
* ***animation-delay*** - Configures the delay between the time the element is loaded and the beginning of the animation sequence.
* ***animation-iteration-count*** - Configures the number of times the animation should repeat; you can specify infinite to repeat the animation indefinitely.
* ***animation-direction*** - Configures whether or not the animation should alternate direction on each run through the sequence or reset to the start point and repeat itself.
* ***animation-fill-mode*** - Configures what values are applied by the animation before and after it is executing.
* ***animation-play-state*** - Lets you pause and resume the animation sequence.
