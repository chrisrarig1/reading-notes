# CSS Transforms, Transitions, and Animations

## Transforms

- The **Transform** property has 2-dimensional and 3-dimensional settings.
Syntax for this property is very simple:
    `element{`
        `transform: wayoftransforming`
    `}`

### 2D vs 3D

- These setups have multiple ways of adjusting an image however they are restricted based on **2D**(x,y) and **3D**(x,y,z) respective planes.

  - **2D**:
    1. *Translate*: Pushes and pulls an element in different directions without disrupting normal flow.
    2. *Skew*: Transforms an element on its horizontal or vertical axis.
    3. *Origin*: This affects the default origin of the element which is its center position.
    4. *Perspective*: This is necessary for a **3D** element to even occur. This allows for a vanishing point. It can be achieved by adjusting the depth and origin values of the element.

  - **3D**:
    1. *Rotate*: Allows for element rotation on its (X,Y,Z) axis
    2. *Scale*: Can be scaled up and down on certain axis
    3. *Translate*: This allows an element to translate relative to a certain axis either getting closer or farther away based on sign value.

## Transitions

- These take place when an element changes its state using pseudo-classes such as: `:hover :focus :active :target`
- Its is typical to use four transition properties: transition-property, transition-duration, transition-timing-function, and transition-delay
  1. *Transition Property*: This is where you would identify what property is changing on the element.
  2. *Transition Duration*: How long will the transformation take until complete. Measured in seconds.
  3. *Transition Timing*: This is the speed in which the transformation will take place.
  4. *Transition Delay*: Timing delay on change.

## Animations

- **Animations** allow for **Transitions** to have multiple states
- **Keyframes** are used to dictate when the animation happens i.e.:

   `keyframes slide {`
  `0% {`
    `left: 0;`
   `top: 0;`
  `}`
  `50% {`
    `left: 244px;`
    `top: 100px;`
  `}`
- Within these **Keyframes** it is possible to manipulate the timing, duration, delay, iteration, and direction of the animation.

# Google Teams

## Finding the perfect team

- Google performed a study to try and develop the perfect team. They viewed their employees daily habits and how it related to productivity.
- Initially the thought was to put like people together. The data was so without pattern that they struggled to prove if this was the case.
- Boosting the collective intelligence is important by allowing shared speaking and shared planning.
- It is important to focus on the feelings of your teammates.
- Groups need to be psychologically safe environments

# Useful Links

- [Transforms](https://learn.shayhowe.com/advanced-html-css/css-transforms/)
- [Transitions/Animations](https://learn.shayhowe.com/advanced-html-css/transitions-animations/)
- [Google Teams](https://www.nytimes.com/2016/02/28/magazine/what-google-learned-from-its-quest-to-build-the-perfect-team.html)