# WEB102 Prework - *Monstern Inc.*

Submitted by: **Sameeraa Kandalgaonkar**

**Monstern Inc.** is a website for the company Sea Monster Crowdfunding that displays information about the games they have funded.

Time spent: **X** hours spent in total

## Required Features

The following **required** functionality is completed:

* [🫶] The introduction section explains the background of the company and how many games remain unfunded.
* [🫶] The Stats section includes information about the total contributions and dollars raised as well as the top two most funded games.
* [🫶] The Our Games section initially displays all games funded by Sea Monster Crowdfunding
* [🫶] The Our Games section has three buttons that allow the user to display only unfunded games, only funded games, or all games.

The following **optional** features are implemented:

 * [🫶] Responsive design that works on desktop and mobile devices
 * [🫶] Hover effects on game cards and buttons for better user interaction
 * [🫶] Dynamic calculation and display of unfunded games count in the introduction
 * [🫶] Proper formatting of numbers with commas for better readability
 * [🫶] Clean card-based layout for individual games with images and descriptions
 * [🫶] Smooth transitions and animations for filtering operations
 * [🫶] Professional styling with custom fonts and color scheme
 * [🫶] Error handling for missing images and data

## Video Walkthrough

<img src='https://raw.githubusercontent.com/SameeraaGKan/web102_prework/main/assets/Screenshot%202025-08-15%20135208.png' title='Video Walkthrough' width='600' alt='Video Walkthrough' />

Here's a walkthrough of implemented features:

<iframe 
    width="600" 
    height="340" 
    src="https://www.youtube.com/embed/BPosCGXX1Nk" 
    title="Video Walkthrough" 
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
    allowfullscreen>
</iframe>

## Notes

### Challenges Encountered

**DOM Manipulation Complexity**: One of the biggest challenges was implementing the filtering system that required complete removal and recreation of game cards. Initially struggled with memory leaks when not properly removing child elements, which was solved by implementing the `deleteChildElements()` function.

**Data Processing and Statistics**: Calculating various statistics (total contributions, funding amounts, unfunded games count) required careful use of JavaScript's `reduce()` method. The challenge was ensuring accurate calculations while maintaining code readability and performance.

**Template Literals and Dynamic Content**: Creating dynamic HTML content using template literals while ensuring proper escaping and handling of missing data (like images) required careful attention to detail and error handling.

**Responsive Design**: Balancing the flexbox layout to work across different screen sizes while maintaining the card-based design was challenging, especially ensuring proper spacing and alignment.

**Event Handling**: Implementing the filtering buttons required understanding event delegation and ensuring that event listeners were properly attached and that the filtering functions correctly updated the DOM.

**Array Methods Mastery**: This project required extensive use of modern JavaScript array methods (`filter()`, `reduce()`, `sort()`) which initially felt overwhelming but became more intuitive through practice.

## Technical Implementation Details

### Key Components Built

**Statistics Dashboard**: Implemented using `reduce()` to calculate total contributions, total funding, and game counts, with `toLocaleString()` for proper number formatting.

**Dynamic Filtering System**: Used `filter()` method combined with DOM manipulation to show/hide games based on funding status, with smooth transitions.

**Game Card Generation**: Created reusable function `addGamesToPage()` that uses template literals to generate consistent card layouts for all games.

**Top Games Ranking**: Implemented sorting algorithm using `sort()` with destructuring assignment to identify and display the highest-funded games.

### Code Organization

The project follows a modular approach with clear separation of concerns:
- Data import and processing
- DOM manipulation functions  
- Event handling and user interactions
- Statistics calculation and display

## Future Enhancements

If given more time, potential improvements could include:
- Search functionality to find specific games
- More detailed game information in modal windows
- User authentication and favorites system
- Real-time funding progress bars
- Integration with actual payment processing
- Advanced sorting options (by date, category, etc.)
- Accessibility improvements (screen reader support, keyboard navigation)

## License

    Copyright [2025] [Sameeraa]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
