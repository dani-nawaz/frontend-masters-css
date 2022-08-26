# Lesson 0: Fundamentals

- Why animate? Guidance and clarification, style and branding.
- Duration: how long an _iteration_ of an animation takes to complete.
- Delay: how long it takes before an animation _starts_
- Timing function: the _easing_ of an animation
- CSS Variables: custom properties that can be inherited by elements and set by JavaScript:
- what to animate: Transform and opacity(great)(GPU accelerated), color and background(umm good)(we have to talk to the browser, we are not moving anything we are triggering paint we are still having 60fps but not if we apply to many elements be carefull), Height width left right etc (a big no)
- Properties like transform and opacity are less expensive to animate because they don't require recalculation of the layout or a repaint. Other properties like height and width require a repaint and negatively impact the performance of the page:(reflowing all the other properties kinda of domino effect).
- if we are not having 60fps the animation would look like jaggy one.
- if we don't have green listing in lighthouse(google performance) then the site drops down in the SEO listing 

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
