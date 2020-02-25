---
##### shortDescription
Registers a set of elements that should be animated as "entering" using the specified animation configuration.

##### param(elements): jQuery
A jQuery object including the elements to be animated.

##### param(animation): animationConfig|String
An object defining the target animation or the name of the animation that is registered in the [animationPresets](/api-reference/50%20Common/utils/animationPresets '/Documentation/ApiReference/Common/Utils/animationPresets') repository.

---
Before [starting](/Documentation/ApiReference/Common/Utils/TransitionExecutor/Methods/#startconfig) a transition (a set of simultaneous animations), the elements that will take part in it and the animation configurations to be used to animate these elements should be registered. For this purpose, use the **enter(elements, animation)** method. The elements registered using this method will be animated as "entering" ones. To register elements for a "leaving" animation within this transition, use the [leave(elements, animation)](/api-reference/50%20Common/utils/TransitionExecutor/3%20Methods/leave(elements_animation).md '/Documentation/ApiReference/Common/Utils/TransitionExecutor/Methods/#leaveelements_animation') method.

If you pass a name of a predefined animation as the second parameter, but an animation is not found by this name in the [animation repository](/api-reference/50%20Common/utils/animationPresets '/Documentation/ApiReference/Common/Utils/animationPresets/'), the specified element(s) will not be animated within this transition.