# vue3typed

## reference
```
https://www.npmjs.com/package/vue-typed-js
https://github.com/Orlandster1998/vue-typed-js#readme
```

## Project setup
```
yarn install
```
### Compiles and hot-reloads for development
```
yarn serve
```

### Install

```
yarn add vue3typed
```

### vue

```vue
<template>
    <vuetyped :string="['Hello World!']">
      <div class="typing"></div>
    </vuetyped>
</template>

<script setup>
import vuetyped from "vue3typed/libs/typed";
</script>
```
### or main.js
```js
import vuetyped from 'vue3typed'
createApp(App).use(vuetyped).mount('#app')
```
### Properties
| Property             | Type    | Description                                                          | Usage                                                           |
|----------------------|---------|----------------------------------------------------------------------|-----------------------------------------------------------------|
| strings              | Array   | strings to be typed                                                  | `:strings="['Text 1', 'Text 2']"` |
| stringsElement       | String  | ID of element containing string children                             | `:stringsElement="'myId'"`                                                                |
| typeSpeed            | Number  | type speed in milliseconds                                           | `:typeSpeed="50"`                                                                |
| startDelay           | Number  | time before typing starts in milliseconds                            | `:startDelay="1000"`                                                                |
| backSpeed            | Number  | backspacing speed in milliseconds                                    | `:backSpeed="10"`                                                                |
| smartBackspace       | Boolean | only backspace what doesn't match the previous string                | `:smartBackspace="true"`                                                                |
| shuffle              | Boolean | shuffle the strings                                                  | `:shuffle="true"`                                                                |
| backDelay            | Number  | time before backspacing in milliseconds                              | `:backDelay="100"`                                                                |
| fadeOut              | Boolean | Fade out instead of backspace                                        | `:fadeOut="true"`                                                                |
| fadeOutClass         | String  | css class for fade animation                                         | `:fadeOutClass="'fadeOutClass'"`                                                                |
| fadeOutDelay         | Number | fade out delay in milliseconds                                       | `:fadeOutDelay="500"`                                                                |
| loop                 | Boolean | loop strings                                                         | `:loop="true"`                                                                |
| loopCount            | Number  | amount of loops                                                      | `:loopCount="3"`                                                                |
| showCursor           | Boolean | show cursor                                                          | `:showCursor="true"`                                                                |
| cursorChar           | String  | character for cursor                                                 | `:cursorChar="'_'"`                                                                |
| autoInsertCss        | Boolean | insert CSS for cursor and fadeOut into HTML                          | `:autoInsertCss="true"`                                                                |
| attr                 | String  | attribute for typing Ex: input placeholder, value, or just HTML text | `:attr="'placeholder'"`                                                                |
| bindInputFocusEvents | Boolean | bind to focus and blur if el is text input                           | `:bindInputFocusEvents="true"`                                                                |
| contentType          | String  | 'html' or 'null' for plaintext                                       | `:contentType="'html'"`   



## Event
You can listen to the following events:

| Event                  | Description                                                          | Usage                                                           |
|------------------------|----------------------------------------------------------------------|-----------------------------------------------------------------|
| onComplete             | All typing is complete                                               | `@onComplete="doSmth()"` |
| preStringTyped         | Before each string is typed                                          | `@preStringTyped="doSmth()"`                                                                |
| onStringTyped          | After each string is typed                                           | `@onStringTyped="doSmth()"`                                                                |
| onLastStringBackspaced | During looping, after last string is typed                           | `@onLastStringBackspaced="doSmth()"`                                                                |
| onTypingPaused         | Typing has been stopped                                              | `@onTypingPaused="doSmth()"`                                                                |
| onTypingResumed        | Typing has been started after being stopped                          | `@onTypingResumed="doSmth()"`                                                                |
| onReset                | After reset                                                          | `@onReset="doSmth()"`                                                                |
| onStop                 | After stop                                                           | `@onStop="doSmth()"`                                                                |
| onStart                | After start                                                          | `@onStart="doSmth()"`                                                                |
| onDestroy              | After destroy                                                        | `@onDestroy="doSmth()"`                                                                |
Use prettier to format
