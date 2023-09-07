# digital-clock

This is a simple digital clock created using HTML, CSS, and JavaScript. It displays the current time in hours, minutes, and seconds, with an AM/PM indicator. The clock is styled on a background image and is positioned in the center of the screen.


## Working

The HTML structure defines a container with five <span> elements: one for hours, minutes, seconds, and AM/PM indicator. These elements are initially set to "00" for hours, minutes, and seconds and "AM" for the session.

In the JavaScript code (index.js), we have a displayTime function that gets the current time using the Date object. It then extracts the hours, minutes, and seconds from this date.

Depending on the value of hrs, it sets the session to "AM" if hrs is less than 12 (before noon) and "PM" otherwise.

If hrs is greater than 12 (after noon), it subtracts 12 from it to display time in the 12-hour format.

Finally, it updates the HTML elements with the current time values.

The setInterval function is used to call the displayTime function every 10 milliseconds, ensuring that the clock updates in real-time.
