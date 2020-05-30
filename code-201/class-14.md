# Reading 14a: CSS Transforms, Transitions, and Animations

### Transforms

* CSS3 brought new ways to position/alter elements with new properties like `transform`

* **Transform** has two different settings - for 2-D and 3-D
  - Each setting has its own properties/values

* Very dynamic, but browser support is still not great for the property at this time

#### Transform Syntax

* Transform properties can be simple, but often include multiple **vendor prefixes** to get better support across all browsers

* Vendor prefixes are strongly encouraged as best-practice for the time being until browser support is more widespread

* Example:

                div {
          -webkit-transform: scale(1.5);
            -moz-transform: scale(1.5);
              -o-transform: scale(1.5);
                  transform: scale(1.5);
        }

#### Examples of Transforms:

* Note: Common for multiple transformed to be used simultaneously 
* To do so, add transform properties/values within the `transform` property, one after the other without using commas

#### 2-D Transforms:
  * `rotate`, `rotateX`, `rotateY`
  * `scale`, `scaleX`, `scaleY`
  * `translate`, `translateX`, `translateY`
  * `skew`, `skewX`, `skewY`
  * `transform-origin`
  * `perspective`
  * `perspective-origin`
  * `scale`
  * `backface-visibility`

### Transitions 

* **Transitions** allow for animations within HTML without the use of JavaScript or Flash
  - CSS3 allows you to alter the look/behavior of an element whenever a **state change** occurs
  - State changes include *hover*, *focus*, *targeted*, and *active*
* Transitions also use vendor prefixes

#### Pseudo-Classes Used for Targeting Transitions
* `:hover`
* `:focus`
* `:active`
* `:target`

#### Transition-Related Properties
* `transition-property`
* `transition-duration`
* `transition-timing-function`
* `transition-delay`


Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)