# Kiwi Trivia Pursuit: Genus Edition

A simple, family-friendly trivia web app with the six classic categories and 800 questions in each (4,800 in total). The questions cover the whole world, with plenty about New Zealand mixed in.

Pick a category, read the question, then flip the switch to see the answer.

## Features

- Six categories: Geography, Entertainment, History, Arts & Literature, Science & Nature, and Sports & Leisure.
- 800 questions per category, at roughly the difficulty of the classic adult edition.
- No repeats: you won't see a question again until you've seen every question in that category. Your progress is saved in the browser, and **↺ Reshuffle** starts again.
- It's plain HTML, CSS and JavaScript: no build step, no server and no dependencies. It works offline once loaded, and also opens straight from your computer (`file://`).

## Files

```
index.html                    the app
questions/geography.js        800 questions each
questions/entertainment.js
questions/history.js
questions/arts-literature.js
questions/science-nature.js
questions/sports-leisure.js
```

## Publishing on GitHub Pages

1. Create a new repository and upload all of these files, keeping the `questions` folder.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then click **Save**.
4. After a minute or so, the app will be live at `https://<your-username>.github.io/<repo-name>/`.

## Editing questions

Each question file is a JavaScript array of entries:

```js
{ "q": "What is New Zealand's highest mountain?", "a": "Aoraki / Mount Cook", "n": "About 3,724 m." }
```

- `q` is the question.
- `a` is the answer.
- `n` is an optional note shown under the answer.

You can add or remove entries freely; the app counts them automatically. Keep a comma between entries. If you remove questions, click **↺ Reshuffle** (or clear the site's stored data) so that saved progress matches the new list.

## A note on accuracy

The questions were written with AI help and then fact-checked: every question was reviewed, and the doubtful or time-sensitive ones were checked against current sources (November 2026). Even so, with 4,800 questions a few errors may remain. Facts that change over time, such as record holders, are correct as of November 2026. If you spot a mistake, fix it in the relevant file.
