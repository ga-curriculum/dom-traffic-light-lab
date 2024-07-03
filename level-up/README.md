# ![Javascript Traffic Light Lab - Level Up](./assets/hero.png)

## Refactoring the Traffic Light Lab

Now that you have a basic solution for the traffic light lab, you may have noticed that the simplest solution isn't very [DRY (Don't Repeat Yourself)](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself).

In this exercise, you'll refactor the existing solution code using `querySelectorAll` and the `forEach` method to ensure all the functionality exists within a single `forEach` callback function.

1. **Refactor Code**:
   - Use `querySelectorAll` to select multiple elements.
   - Use the `forEach` method to iterate over these elements and implement the traffic light functionality in a single callback function.

### Hints and Tips

- **Ordered Collections**:
  - Arrays in JavaScript are **ordered** collections of data. Use this to your advantage.

- **forEach Callback**:
  - The callback function for `forEach` is called with three arguments:
    - `element`: The current element in the iteration.
    - `index`: The index of the current element.
    - `array`: The array that `forEach` was called on.
  - The `index` can be useful for associating the current button with a specific bulb.

- **Dynamic Color Setting**:
  - To set the color of a bulb dynamically based on the index of the current button, consider using another array.

Good Luck! 🚦
