# Number Identification Game (Extra Practice with "2")

A simple, web-based game designed to help young learners (around 6 years old) practice recognizing numbers in the range **10 to 99**, with extra focus on the digit **"2"**. This version **does not** use any external API (like GIPHY)—instead, it displays a **static dancing figure** upon a correct answer.

## Features

1. **Strong Focus on '2'**  
   - **70%** of the time, the game picks a number containing the digit “2.”  
   - Distractor answers also frequently contain “2.”  

2. **Reversed Number Distractor**  
   - If the correct number is, for example, **25**, a distractor will be **52** (unless they are the same, like **11**).

3. **Four Multiple-Choice Options**  
   - One correct answer, and three distractors.  
   - Large, kid-friendly buttons.

4. **Score & Errors**  
   - Correct answers add a **flower** (🏵️) to your score.  
   - Wrong answers add a **pink flower** (🌸) to the error counter.  
   - Score and error counts are saved in the URL, so refreshing does not reset progress.

5. **Cute Dancing Figure**  
   - A **static** animated GIF is displayed upon a correct answer, bouncing via CSS animations.

6. **Speech Synthesis**  
   - The game uses the browser’s built-in Speech Synthesis API to read aloud the number that the child must identify.

7. **No-Cache Meta Tags**  
   - Encourages the browser to fetch the newest version of the game rather than a cached copy.

## Getting Started

1. **Visit the Game**  
   - Simply go to [https://ori226.github.io/aviv_count/](https://ori226.github.io/aviv_count/) in a modern browser (Chrome, Firefox, Safari, Edge, etc.).  
2. **Play** by clicking **"Play Number"** to hear a number, then pick the correct multiple-choice option.

## Usage

1. **Play Number**  
   - Click the "Play Number" button to hear the spoken number (e.g., "25").  
2. **Choose an Answer**  
   - Select one of the four large buttons (numbers).  
   - If correct, you’ll see a **“Good job!”** message, a dancing figure, and your score goes up.  
   - If wrong, you get an “Oops!” message and an error gets recorded.  
3. **Next Number**  
   - Click "Next Number" to load another random question.

## Customization

- **Probability of '2'**  
  - Look for the line `const shouldPick2 = Math.random() < 0.7;` in the script and change `0.7` to another value.  
- **Range of Numbers**  
  - By default, we pick numbers between **10** and **99**. Change the loop in the JavaScript if you want a different range.  
- **Dancing Figure**  
  - The code references a GIF in an `<img>` tag (`<img id="dancingFigure" src="...">`).  
  - Swap out the `src` URL to any other static or animated image you prefer.  
- **Styling**  
  - All layout, colors, and animations live in the `<style>` block. Adjust as desired.

## Troubleshooting

- **Speech Synthesis Not Working**  
  - Ensure you’re using a browser that supports the Web Speech API. Most modern desktop and mobile browsers do.  
- **Caching**  
  - We include meta tags to reduce caching. If the browser still serves an older version, try opening in a private/incognito window or rename your HTML file.

## License

Use this code freely for educational or personal projects. If you want to open-source it, consider adding an [MIT License](https://opensource.org/licenses/MIT) or similar.

---

**Enjoy practicing numbers with your child**—especially mastering **"2"**!
