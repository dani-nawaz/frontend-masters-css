# Lesson 0: Fundamentals

- Why animate? Guidance and clarification, style and branding.
- Duration: how long an _iteration_ of an animation takes to complete.
- Delay: how long it takes before an animation _starts_
- Timing function: the _easing_ of an animation
- CSS Variables: custom properties that can be inherited by elements and set by JavaScript:
- what to animate: Transform and opacity(great), color and background(umm good), Height width left right etc (a big no)
- Properties like transform and opacity are less expensive to animate because they don't require recalculation of the layout or a repaint. Other properties like height and width require a repaint and negatively impact the performance of the page.

```css
:root {
  --duration: 2s;
}

.thing {
  animation-duration: calc(var(--duration, 1s));
}
```

```js
const thingEl = document.querySelector('.thing');

thingEl.style.setProperty('--color', 'green');
```

## Resources

- [Ground Rules for CSS Animations](https://css-tricks.com/ground-rules-for-web-animations/)
- [UX Animation Principles: Duration](https://codepen.io/team/keyframers/pen/gdJJZV)
- [UX Animation Principles: Stagger](https://codepen.io/team/keyframers/pen/GXaaNw)
- [UX Animation Principles: Acceleration](https://codepen.io/team/keyframers/pen/ZqbWao)
