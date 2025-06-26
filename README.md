# Kitboga Code Jam - XKCD 2228 Inspired Captcha

A simple "select all the images" captcha inspired by XKCD #2228 for the [2025 Kitboga Code Jam](https://kitboga.com/codejam)

![More likely: Click on all the pictures of people who appear disloyal to (name of company or government)](https://imgs.xkcd.com/comics/machine_learning_captcha.png)

Includes some fun questions like:
* Select all the images that make you feel a vague sense of existential dread.

## How It Works

* Includes 5 randomized captchas
* You must get 3 correct to continue (configurable)
* Captchas are repeated if you get all of them wrong, but each captcha includes 4 versions of each image (randomly selected each time)
* All answers can be found in [./captcha/captchas.json](./captcha/captchas.json)

## Configuration

Update the config values at the top of the script:

```js
const CONSTANTS = {
  CONFIG: {
    REQUIRED_CORRECT: 3, // The number of prompts that must be correct to pass
    PROMPT_FADE_DELAY: 200, // The delay before the prompt fades in
    CHECKING_DELAY: 2000, // The delay before the next captcha is loaded
  }
};
```

Try it out here: [https://w3cj.github.io/kitboga-codejam25-xkcd-captcha/](https://w3cj.github.io/kitboga-codejam25-xkcd-captcha/)