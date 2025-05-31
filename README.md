# Simple Counter App

A basic web application that allows users to increment a numerical counter. This project demonstrates fundamental HTML, CSS (with Tailwind CSS), and JavaScript concepts.

## Project Overview

The application displays a counter, initialized at 0, and an "Increment" button. Each click on the button increases the counter's value by one.

## Features

* **Counter Display:** Shows the current count.
* **Increment Button:** Increases the count when clicked.
* **Simple & Clean UI:** Styled with Tailwind CSS for a modern look and feel.

## Technologies Used

* **HTML:** Structures the content of the web page.
* **CSS (Tailwind CSS):** Styles the application for visual appeal and responsiveness. Tailwind CSS is loaded via a CDN.
* **JavaScript:** Implements the counter logic and button functionality.

## How to Run

1.  **Save the Code:** Copy the HTML code from the `simple_counter_app` (or save it as an `index.html` file).
2.  **Open in Browser:** Open the `index.html` file in any modern web browser (e.g., Chrome, Firefox, Safari, Edge).

No special build steps or dependencies are required beyond a web browser, as Tailwind CSS is included via a CDN.

## Code Structure

* **`index.html` (or the provided HTML block):**
    * **`<head>`:**
        * Includes metadata, the title of the page, and a link to the Tailwind CSS CDN.
        * Contains a `<style>` block for any potential custom CSS (though primarily uses Tailwind).
    * **`<body>`:**
        * Contains the main content of the application, centered on the page.
        * A `div` element acts as a container for the counter's heading, display area, and button.
        * The counter value is displayed in a `<p>` tag with the ID `countDisplay`.
        * The increment functionality is triggered by a `<button>` with the ID `incrementButton`.
    * **`<script>`:**
        * Located at the end of the `<body>` to ensure HTML elements are loaded before the script runs.
        * **`countDisplay`:** A constant that references the paragraph element where the count is shown.
        * **`incrementButton`:** A constant that references the button element.
        * **`count`:** A variable initialized to `0` to store the current counter value.
        * **`updateDisplay()`:** A function that updates the `textContent` of `countDisplay` with the current `count`.
        * **Event Listener:** An event listener is attached to `incrementButton`. On a 'click' event:
            * The `count` is incremented (`count++`).
            * `updateDisplay()` is called to reflect the new count on the page.

## Future Enhancements (Optional)

* Add a "Decrement" button.
* Add a "Reset" button to set the counter back to 0.
* Allow users to set a custom increment/decrement step.
* Persist the count using `localStorage` so it's remembered across browser sessions.
