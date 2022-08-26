# Lesson 4: States

- Determining states for animation
- [Data attributes](https://developer.mozilla.org/en-US/docs/Learn/HTML/Howto/Use_data_attributes)
- ![Screenshot 2022-08-26 at 4 27 42 PM](https://user-images.githubusercontent.com/69709106/186893810-384609aa-74c7-4cb2-8ba6-7e2e918e0196.png)
- if we prefix an attribute with data then we can access it with the dataset.
- this make it very usefull to work b/w JS, CSS 
- Creating simple state machines
-  A state machine is a JavaScript Object with properties matching each state value and event declarations indicating which state should be returned given a certain event.
- using states we can assign diff animations WRT diff states

## Exercise

- Use JavaScript to change the state of the form from `'subscribe'` to `'loading'` when the button is clicked.
- Afte r 2 seconds in `'loading'`, change the state to `'success'` or `'error'` (chosen randomly to simulate an error state)
  - Hint: use `Math.random() < 0.5`
- On the `'error'` state, animate the form by shaking it
  - You will need to create a `shake` animation with `@keyframes`
- Refactor to a state machine to send events and prevent impossible state transitions (we'll do this together)

## Resources

- [Expanding Video Player](https://codepen.io/team/keyframers/pen/dLjZEO)
- [Contact Form Transitions](https://codepen.io/team/keyframers/pen/YzwGZwN)
- [Password Modal](https://codepen.io/davidkpiano/pen/WKvPBP)
