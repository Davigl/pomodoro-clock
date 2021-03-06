<h1 align="center">
  <img alt="⌛️ React React Pomodoro Clock" src="https://i.imgur.com/3JGmXWy.png" />
  <br>
</h1>

<p align="center">
  <a href="https://github.com/Davigl/pwa-pomodoro-clock/commits/master">
    <img alt="GitHub Last Commit" src="https://img.shields.io/github/last-commit/Davigl/pwa-pomodoro-clock?style=flat-square&color=ff69b4">
  </a>
  
  <a href="https://github.com/Davigl/pwa-pomodoro-clock/stargazers">
    <img alt="GitHub Stars" src="https://img.shields.io/github/stars/Davigl/pwa-pomodoro-clock?style=flat-square&color=9cf">
  </a>

  <a href="https://github.com/Davigl/pwa-pomodoro-clock/issues">
    <img alt="Repository issues" src="https://img.shields.io/github/issues/Davigl/pwa-pomodoro-clock?style=flat-square&color=yellow">
  </a>
  
  <img alt="GitHub top Language" src="https://img.shields.io/github/languages/top/davigl/pwa-pomodoro-clock.svg?style=flat-square">

  <img alt="Repository Size" src="https://img.shields.io/github/repo-size/Davigl/pwa-pomodoro-clock?style=flat-square&color=blueviolet">
</p>

<p align="center">
  <a href="#thinking-about">About</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#user-content--user-stories">Stories</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#memo-license">License</a>
</p>

## :thinking: About

Pomodoro Clock is a flexible and easy to use online Pomodoro Technique Timer. This technique uses a timer to break down work into intervals, traditionally 25 minutes in length, separated by short breaks. Visit the project by clicking [here](https://eudavi-pomodoro-timer.netlify.com/).

<div align="center">

![](https://i.imgur.com/mzsHotL.gif)

*Pomodoro Clock*

</div>

## 🦹‍ User Stories 

- [x] <strong>User Story #1:</strong> I can see an element with <code>id="break-label"</code> that contains a string (e.g. "Break Length").   
- [x] <strong>User Story #2:</strong> I can see an element with <code>id="session-label"</code> that contains a string (e.g. "Session Length").   
- [x] <strong>User Story #3:</strong> I can see two clickable elements with corresponding IDs: <code>id="break-decrement"</code> and <code>id="session-decrement"</code>.   
- [x] <strong>User Story #4:</strong> I can see two clickable elements with corresponding IDs: <code>id="break-increment"</code> and <code>id="session-increment"</code>.   
- [x] <strong>User Story #5:</strong> I can see an element with a corresponding <code>id="break-length"</code>, which by default (on load) displays a value of 5.
- [x] <strong>User Story #6:</strong> I can see an element with a corresponding <code>id="session-length"</code>, which by default displays a value of 25.
- [x] <strong>User Story #7:</strong> I can see an element with a corresponding <code>id="timer-label"</code>, that contains a string indicating a session is initialized (e.g. "Session").   
- [x] <strong>User Story #8:</strong> I can see an element with corresponding <code>id="time-left"</code>. NOTE: Paused or running, the value in this field should always be displayed in <code>mm:ss</code> format (i.e. 25:00).   
- [x] <strong>User Story #9:</strong> I can see a clickable element with a corresponding <code>id="start_stop"</code>.   
- [x] <strong>User Story #10:</strong> I can see a clickable element with a corresponding <code>id="reset"</code>.   
- [x] <strong>User Story #11:</strong> When I click the element with the id of <code>reset</code>, any running timer should be stopped, the value within <code>id="break-length"</code> should return to <code>5</code>, the value within <code>id="session-length"</code> should return to 25, and the element with <code>id="time-left"</code> should reset to it's default state.   
- [x] <strong>User Story #12:</strong> When I click the element with the id of <code>break-decrement</code>, the value within <code>id="break-length"</code> decrements by a value of 1, and I can see the updated value.   
- [x] <strong>User Story #13:</strong> When I click the element with the id of <code>break-increment</code>, the value within <code>id="break-length"</code> increments by a value of 1, and I can see the updated value.   
- [x] <strong>User Story #14:</strong> When I click the element with the id of <code>session-decrement</code>, the value within <code>id="session-length"</code> decrements by a value of 1, and I can see the updated value.   
- [x] <strong>User Story #15:</strong> When I click the element with the id of <code>session-increment</code>, the value within <code>id="session-length"</code> increments by a value of 1, and I can see the updated value.   
- [x] <strong>User Story #16:</strong> I should not be able to set a session or break length to <= 0.   
- [x] <strong>User Story #17:</strong> I should not be able to set a session or break length to > 60.   
- [x] <strong>User Story #18:</strong> When I first click the element with <code>id="start_stop"</code>, the timer should begin running from the value currently displayed in <code>id="session-length"</code>, even if the value has been incremented or decremented from the original value of 25.   
- [x] <strong>User Story #19:</strong> If the timer is running, the element with the id of <code>time-left</code> should display the remaining time in <code>mm:ss</code> format (decrementing by a value of 1 and updating the display every 1000ms).   
- [x] <strong>User Story #20:</strong> If the timer is running and I click the element with <code>id="start_stop"</code>, the countdown should pause.   
- [x] <strong>User Story #21:</strong> If the timer is paused and I click the element with <code>id="start_stop"</code>, the countdown should resume running from the point at which it was paused.   
- [x] <strong>User Story #22:</strong> When a session countdown reaches zero (NOTE: timer MUST reach 00:00), and a new countdown begins, the element with the id of <code>timer-label</code> should display a string indicating a break has begun.   
- [x] <strong>User Story #23:</strong> When a session countdown reaches zero (NOTE: timer MUST reach 00:00), a new break countdown should begin, counting down from the value currently displayed in the <code>id="break-length"</code> element.   
- [x] <strong>User Story #24:</strong> When a break countdown reaches zero (NOTE: timer MUST reach 00:00), and a new countdown begins, the element with the id of <code>timer-label</code> should display a string indicating a session has begun.   
- [x] <strong>User Story #25:</strong> When a break countdown reaches zero (NOTE: timer MUST reach 00:00), a new session countdown should begin, counting down from the value currently displayed in the <code>id="session-length"</code> element.   
- [x] <strong>User Story #26:</strong> When a countdown reaches zero (NOTE: timer MUST reach 00:00), a sound indicating that time is up should play. This should utilize an HTML5 <code>audio</code> tag and have a corresponding <code>id="beep"</code>.   
- [x] <strong>User Story #27:</strong> The audio element with <code>id="beep"</code> must be 1 second or longer.   
- [x] <strong>User Story #28:</strong> The audio element with id of <code>beep</code> must stop playing and be rewound to the beginning when the element with the id of <code>reset</code> is clicked.   

## :memo: License

Copyright © 2020, [Davi Guimarães](https://github.com/davigl).
