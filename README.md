# Sass Component Template

A template to help create consistent, performant Sass components.

## Comment Detail

The ordering of these is intentional. These groupings leverage the cascade to make the partials as efficient as possible.

- [`01`](https://github.com/ericwbailey/sass-component-template/blob/master/_type.name.scss#L1) Provides an 80 character-wide column marker
- [`02`](https://github.com/ericwbailey/sass-component-template/blob/master/_type.name.scss#L2) Category type: Layout, Object, Component, Theme, etc.
- [`03`](https://github.com/ericwbailey/sass-component-template/blob/master/_type.name.scss#L3) This is the partial's name spelled out as a proper noun
- [`04`](https://github.com/ericwbailey/sass-component-template/blob/master/_type.name.scss#L4) A link to the partial on a living styleguide, if available
- [`08`](https://github.com/ericwbailey/sass-component-template/blob/master/_type.name.scss#L8) Use this comment block to provide any high level background information about the partial. Can span multiple lines, is constrained to an 80 character-long width. May be replaced with [SassDoc](http://sassdoc.com/)
- [`13`](https://github.com/ericwbailey/sass-component-template/blob/master/_type.name.scss#L13) Update to reflect the component's type and name. For example, a layout partial's class name would be called `.l-sidebar`
- [`14`](https://github.com/ericwbailey/sass-component-template/blob/master/_type.name.scss#L14) [Encapsulated logic](https://www.devbridge.com/articles/7-sass-techniques-to-help-you-write-better-code/) prevents unpredictable behavior
- [`15`](https://github.com/ericwbailey/sass-component-template/blob/master/_type.name.scss#L15) Variables can be used for all subsequent logic
- [`19`](https://github.com/ericwbailey/sass-component-template/blob/master/_type.name.scss#L19) Use extends with [a healthy dose of discretion](http://csswizardry.com/2016/02/mixins-better-for-performance/)
- [`21`](https://github.com/ericwbailey/sass-component-template/blob/master/_type.name.scss#L21) Group properties alphabetically by intent. Use an empty space between each property grouping for easier scanning
- [`26`](https://github.com/ericwbailey/sass-component-template/blob/master/_type.name.scss#L26) `cursor`, `transition`, etc.
- [`28`](https://github.com/ericwbailey/sass-component-template/blob/master/_type.name.scss#L28) Pseudo classes can inform pseudo elements, therefore they come first
- [`37`](https://github.com/ericwbailey/sass-component-template/blob/master/_type.name.scss#L37) Use HTML (ex: `[hidden]`) and ARIA (ex: `[aria-busy="true"]`) attributes to provide [meaningful, semantic states](https://css-tricks.com/user-facing-state/)
- [`39`](https://github.com/ericwbailey/sass-component-template/blob/master/_type.name.scss#L39) Use Sass' ampersand selector to modify the partial's presentation based on a class declared higher up in the DOM. This is useful for theming and modifying behavior based on state. Ex: `.t-dark & { … }`
- [`42`](https://github.com/ericwbailey/sass-component-template/blob/master/_type.name.scss#L42) Although [`@supports`](https://www.lottejackson.com/learning/supports-will-change-your-life) is technically not a media query, it is very similar behavior-wise
- [`43`](https://github.com/ericwbailey/sass-component-template/blob/master/_type.name.scss#L43) Feature queries include Reduced Motion, High Contrast Mode, etc.
- [`44`](https://github.com/ericwbailey/sass-component-template/blob/master/_type.name.scss#L44) Be sure to develop partials mobile first. I find a library like [mappy-breakpoints](https://github.com/zellwk/mappy-breakpoints) helps to manage breakpoints and tweakpoints. After declaring a breakpoint, be sure to follow this template's ordering within the breakpoint
- [`46`](https://github.com/ericwbailey/sass-component-template/blob/master/_type.name.scss#L46) Sass' ampersand selector works really well with a BEM naming methodology. Be sure be sure to follow this template's ordering within the nested selectors. Try not to nest selectors more than 3 deep—if you find yourself doing so, you can probably refactor


## Notes
- I prefer to use a comment as a subsection heading. I find it helps making scanning the file easier