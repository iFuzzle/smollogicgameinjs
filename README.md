# SmolLogicGameInJS
SmolLogicGameInJS is a compact, JavaScript-based logic puzzle game, drawing inspiration from the classic mastermind game. It is designed to offer solvability through hints and is intended for integration as a subpage within a larger system.

## Getting Started
To run the game, you can either open the `GamePage.html` file locally or host it on a server. While the current version lacks CSS and visual enhancements, it's recommended to build upon the base code to enhance its visual appeal.

## Game Configuration
Although the system is relatively straightforward to modify, its primary goal is to remain simple and seamlessly integrate into existing environments. You can easily adjust the number of rows and columns for the hints by modifying the values within the array. Note that there is currently no validation to ensure uniform row lengths, which might lead to untested edge cases.

Example:
```JavaScript
Copy code
hints = [
  [0,0,0,0],
  [0,0,0,1],
  [0,0,1,0],
  [0,1,0,0]
];

correct = [
  [1,0,0,0]
];
```
In this example, the game generates four rows of hints, gradually progressing from "0,0,0,0" to "1,0,0,0" in each row. Players need to interact with the buttons to align them with the desired logic, such as `[1][0][0][0]`. Upon clicking the check button, the values are evaluated. Incorrect combinations trigger a popup alert, while a correct solution leads to redirection (e.g., advancing to the next level or a celebratory YouTube video).

## Acknowledgements
I extend my gratitude to R.K.H. for the request to develop this game and for granting permission to release it under my name. The initial version was completed in approximately two hours.

## Future Enhancements
Contributions to further evolve this project are welcomed through forks or pull requests. Several ideas and requests have already emerged:

- Enable button values beyond two options
- Develop a dedicated page to generate and validate inputs
- Allow multiple rows in the answer (currently limited to `correct[0]`)
- Enhance the visual presentation:
  - Ensure button width matches that of `td` elements
  - Introduce CSS improvements
    - Bonus points for incorporating Star Trek aesthetics!
