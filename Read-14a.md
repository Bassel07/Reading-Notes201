# CSS Transforms, Transitions, and Animations

CSS gives us two primary ways of animating elements. Transition and transform manipulate from one state to another,
while animation paired with @keyframes rules can set multiple style rules at various points throughout the animation duration.

![img](https://webdesignerwall.com/wp-content/uploads/2017/01/transforms.jpg)

# Transforms

Example:
![image](https://user-images.githubusercontent.com/85109819/124994450-bbc4ff80-dffa-11eb-9b09-88af19bfdfbe.png)


Definition and Usage
The transform property applies a 2D or 3D transformation to an element. This property allows you to rotate, scale, move, skew, etc., elements.


# CSS Transitions

CSS transitions allows you to change property values smoothly, over a given duration.

How to Use CSS Transitions?
To create a transition effect, you must specify two things:

* the CSS property you want to add an effect to
* the duration of the effect

![image](https://user-images.githubusercontent.com/85109819/124993919-e2366b00-dff9-11eb-9fb1-5356959fcef2.png)

The transition effect will start when the specified CSS property (width) changes value.

Now, let us specify a new value for the width property when a user mouses over the <div> element:
  
  ![image](https://user-images.githubusercontent.com/85109819/124993964-f4180e00-dff9-11eb-8c08-f32019653982.png)

  
  
 ## Change Several Property Values
  
  The following example adds a transition effect for both the width and height property,
  with a duration of 2 seconds for the width and 4 seconds for the height:
  
  ![image](https://user-images.githubusercontent.com/85109819/124994049-190c8100-dffa-11eb-906e-7a4fe5279f68.png)
  
  The following example shows some of the different speed curves that can be used:
  
  ![image](https://user-images.githubusercontent.com/85109819/124994148-41947b00-dffa-11eb-9dcd-e6f2687904a8.png)

  
  Delay the Transition Effect
  
  The transition-delay property specifies a delay (in seconds) for the transition effect.

The following example has a 1 second delay before starting:
  
  ![image](https://user-images.githubusercontent.com/85109819/124994203-583ad200-dffa-11eb-85ef-c182931d22c0.png)
  
  # Transition + Transformation
  
  The following example adds a transition effect to the transformation:
  
  ![image](https://user-images.githubusercontent.com/85109819/124994288-7acceb00-dffa-11eb-8db2-c6cb76f26890.png)
  
  More Transition Examples
  
  ![image](https://user-images.githubusercontent.com/85109819/124994349-9506c900-dffa-11eb-8c84-6f31091c7b4d.png)
  
  
  # Animations
  
  What are CSS Animations?
  
  An animation lets an element gradually change from one style to another.

You can change as many CSS properties you want, as many times as you want.

To use CSS animation, you must first specify some keyframes for the animation.

Keyframes hold what styles the element will have at certain times.

# The @keyframes Rule
  
  When you specify CSS styles inside the @keyframes rule, the animation will gradually change from the current style to the new style
  at certain times.

To get an animation to work, you must bind the animation to an element.

The following example binds the "example" animation to the <div> element. The animation will last for 4 seconds,
  and it will gradually change the background-color of the <div> element from "red" to "yellow":
  
  ![image](https://user-images.githubusercontent.com/85109819/124994748-2a09c200-dffb-11eb-84a3-320d0b6aa17d.png)

  Note: The animation-duration property defines how long an animation should take to complete. If the animation-duration property is not specified, 
  no animation will occur, because the default value is 0s (0 seconds). 

In the example above we have specified when the style will change by using the keywords "from" and "to" (which represents 0% (start)
  and 100% (complete)).

It is also possible to use percent. By using percent, you can add as many style changes as you like.

The following example will change the background-color of the <div> element when the animation is 25% complete, 
  50% complete, and again when the animation is 100% complete:

  ![image](https://user-images.githubusercontent.com/85109819/124994880-676e4f80-dffb-11eb-8e4f-ff526f21afef.png)
  
  The following example will change both the background-color and the position of the <div> element when the animation is 25% complete,
  50% complete, and again when the animation is 100% complete:
  
  ![image](https://user-images.githubusercontent.com/85109819/124994931-7b19b600-dffb-11eb-840e-1dc7a990be07.png)
  
  # Delay an Animation
  
  The animation-delay property specifies a delay for the start of an animation.

The following example has a 2 seconds delay before starting the animation:
  
  ![image](https://user-images.githubusercontent.com/85109819/124995015-91277680-dffb-11eb-8cf2-feee66b023cb.png)
  
  Set How Many Times an Animation Should Run
  
  ![image](https://user-images.githubusercontent.com/85109819/124995084-aa302780-dffb-11eb-8a2d-c9a443ad09c0.png)
  
  Example
  
  ![image](https://user-images.githubusercontent.com/85109819/124995118-b74d1680-dffb-11eb-9e46-dfe787df87a5.png)
  
  https://www.w3schools.com/css/css3_animations.asp
  
  







