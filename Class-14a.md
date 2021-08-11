#  CSS Transforms, Transitions, and Animations

## Transforms 

```
With CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the transform property. The transform property comes in two different settings, two-dimensional and three-dimensional.

Within this lesson we’ll take a look at both two-dimensional and three-dimensional transforms. Generally speaking, browser support for the transform property isn’t great, but it is getting better every day.

The un-prefixed declaration comes last to overwrite the prefixed versions, should a browser fully support the transform property. We’ll start by discussing how to transform elements on a two-dimensional plane, and then work our way into three-dimensional transforms.

- Scale Demo

The scaleX value will scale the width of an element while the scaleY value will scale the height of an element. To scale both the height and width of an element but at different sizes, the x and y axis values may be set simultaneously.

Using the translateX value will change the position of an element on the horizontal axis while using the translateY value will change the position of an element on the vertical axis. Positive values will push an element down and to the right of its default position while negative values will pull an element up and to the left of its default position.

Using the skewX value distorts an element on the horizontal axis while the skewY value distorts an element on the vertical axis. To distort an element on both axes the skew value is used, declaring the x axis value first, followed by a comma, and then the y axis value.

- Combining Transforms Demo

Using the rotate, scale, transition, and skew values provide an easy way to establish this matrix. However, should you be mathematically inclined, and prefer to take a deeper dive into transforms, try your hand at using the matrix property. 2D Cube Demo.



As previously mentioned, the default transform origin is the dead center of an element, both 50% horizontally and 50% vertically. To change this default origin position the transform-origin property may be used. The transform-origin property can accept one or two values. If two values are specified, the first is used for the horizontal axis and the second is used for the vertical axis.



Since both of them are attempting to position the element, their values can collide. The perspective of an element can be set in two different ways. One way includes using the perspective value within the transform property on individual elements, while the other includes using the perspective property on the parent element residing over child elements being transformed. Using the perspective value within the transform property works great for transforming one element from a single, unique perspective.

When you want to transform a group of elements all with the same perspective, or vanishing point, apply the perspective property to their parent element.

```

##  Transitions & Animations

```
Transitions provide a change from one state to another, while animations can set multiple points of transition upon different keyframes.

Transitions

There are four transition related properties in total, including transition-property, transition-duration, transition-timing-function, and transition-delay. Not all of these are required to build a transition, with the first three are the most popular. In the example below the box will change its background color over the course of 1 second in a linear fashion.

Vendor Prefixes

The code above, as with the rest of the code samples in this lesson, are not vendor prefixed.

The transition-property property determines exactly what properties will be altered in conjunction with the other transitional properties. In the example above, the background property is identified in the transition-property value.

Transition Duration

The duration in which a transition takes place is set using the transition-duration property. The value of this property can be set using general timing values, including seconds and milliseconds . As with the transition-property property value, multiple durations can be declared using comma separated values.

Vendor Prefixing the Keyframe Rule

The animation above is named slide, stated directly after the opening @keyframes rule. The different keyframe breakpoints are set using percentages, starting at 0% and working to 100% with an intermediate breakpoint at 50%. The keywords from and to could be used in place of 0% and 100% if wished. Consider how you might move an element from top to bottom for example.

Once you have declared the animation-name property on an element, animations behave similarly to transitions. To start, animations need a duration declared using the animation-duration property. The animation below should cause the ball to bounce once while moving to the left, however only when hovering over the stage. .stage {.

Animation Fill Mode

The animation-fill-mode property accepts four keyword values, including none, forwards, backwards, and both. The none value will not apply any styles to an element before or after an animation has been run. The backwards value will apply the styles within the first specified keyframe as soon as being identified, before the animation has been run. This does include applying those styles during any time that may be set within an animation delay.

The backwards value may also be affected by the animation-direction property value


```

