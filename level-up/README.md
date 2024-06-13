# ![Traffic Light Lab - Level Up](./assets/hero.png)

You may have noticed that the simplest solution for this traffic light lab isn't very [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself).

Using `querySelectorAll` and the `forEach` method, refactor the existing solution code so that all of the functionality exists within a single `forEach` callback function. 

Take some time to think through this challenge and play around with the code. The following hints are provided in case you get stuck: 

### Hints

- This solution will make use of the fact that arrays in JavaScript are __ordered__ collections of data.

- The callback function for a `forEach` method is called with the following arguments: `element` (the current element in the iteration), `index` (the index of the current element), and `array` (the array that `forEach` was called on). Having access to the `index` might be helpful, if you were trying to associate the current button with a specific bulb. 

- To dynamically set the color of a bulb based on the index of the current button, you could potentially explore the use of another array... 