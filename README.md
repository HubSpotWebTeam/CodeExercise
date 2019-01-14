# HubSpot Web Team Exercise - Instructions

## Setup

1. Clone or download this repository (do not fork it).
2. Install [Node.js](https://nodejs.org/en/download/) and then run `npm install` on your project. We've included recommended packages in `package.json` for you to use, but feel free to add or remove any packages.
3. Set up a build tool (Gulp, WebPack, Grunt, etc.) to compile from the existing `/src` folder to a `/build` directory and run your site locally. If you prefer Gulp, we've included recommended tasks in `gulpfile.js` for you to use, but that file can be modified as much as you see fit.

If everything is set up properly, anyone should be able to fork your project, run `npm install`, and issue a start command (we recommend `npm start`) command from the command line to run your build tool and view your site from `localhost`.

**Spending too much time on step #3?** Skip it and focus on the exercises. When you submit your final assessment, please let us know why you skipped this build tool setup step in the `submission.md` file.

---

## Mockups

This code assessment is broken up into two exercises. All exercises should display on the same page.

### Mockup with collapsed filter

The mockup with all filters collapsed. See the section below for how the expanded filter dropdowns should appear.

<a href="https://cdn2.hubspot.net/hubfs/53/web_team/web-team-test/web-team-exercise_3_v2.png" target="_blank">
    <img src="https://cdn2.hubspot.net/hubfs/53/web_team/web-team-test/web-team-exercise_3.png" alt="Mockup" width="600" />
</a>

#### Mockup with expanded filter

Note the filter dropdown outlined in red.

<a href="https://cdn2.hubspot.net/hubfs/53/web_team/web-team-test/web-team-exercise-v2_expanded.png" target="_blank">
    <img src="https://cdn2.hubspot.net/hubfs/53/web_team/web-team-test/web-team-exercise-v2_expanded.png" alt="Mockup_Hover" width="600" />
</a>

---

## Requirements

1. Without adding or removing HTML elements, style each of the following modules to match the above mockup. Fonts have been provided for you and can be found in the accompanying `/src/views/partials/_fonts.ejs` file. Do not add or remove any of the HTML elements in the `/src/views/partials/_testimonial.ejs` or `/src/views/partials/_filterable-content.ejs` files. You may add attributes to the existing HTML elements, but don't add or remove any DOM elements, and don't edit a DOM element's tag name. Feel free to use CSS pseudoelements. All other files may be edited (e.g. `/src/views/pages/index.ejs`).
2. The page should be responsive. Use your best judgment for how narrow viewports should look.
3. Don't use any CSS frameworks (e.g. Bootstrap). You should use a preprocessor, such as Sass.
4. Focus on writing clean, reusable code.
5. While all the modules should be styled to match the mockup, some require some additional functionality:

   - **Exercise 1 - Filterable Content:**
     1. Use the provided `/src/js/data/data.json` file to generate filterable categories as well as the individual content elements within the `/src/views/partials/_filterable-content.ejs` HTML. The items should be alphabetized by title.
     2. **Dropdowns:** If multiple checkboxes are checked (e.g. _Mystery_ and _Drama_), items from **_both_** categories should display (e.g. all items tagged with either _Mystery_ or _Drama_).
     3. The `Clear Filters` functionality is mandatory.
   - **Exercise 2 - Testimonial Block:**
     1. When clicking `Tell Me More`, fetch text from an API of your choice and update the text within the quote to the left of `Tell Me More`. We recommend [the Random Quotes API](https://talaikis.com/api/quotes/random/), but there are other fun APIs like the [Chuck Norris jokes API](http://www.icndb.com/api/). We're flexible.

6. Have fun with it! If you get stuck, that's OK. Get as far as you can.
7. Before submitting, answer the questions in `submission.md`.

#### Bonus Points

Want an extra challenge? Add some pizzazz to your page. **Note:** These steps are optional, but encouraged. :star2:

1. Feeling particularly good? Use ES6, React, or Vue components.
2. Replace Gulp and use WebPack as your build tool.
3. Add a search field and functionality to the filter module (example in mockup).
4. Add some of your favorite node modules to the project, or modify your build tool with anything that strikes your fancy.
5. Add linting.

#### Grading

We recommend focusing on `Exercise 1 — Filterable Content` as it is graded more heavily. It's a good indicator of your attention to user experience and how you approach data puzzles.

`Exercise 2 — Testimonial Block` is a more of a CSS challenge, so being visually precise while not touching the markup is key.

Remember the `submission.md` file — this is your chance to tell us what you thought about the activity and what else you would have done. It's a good way for us to get to know you and your process. We want to hear from you!

## Submission

Be sure to fill out the `submission.md` file before submitting. Once complete, email either a) a zip of your work or b) a link to your GitHub repository to your recruiting specialist so they can send to the team.

---

## FAQs

<details>
    <summary><strong>When is the exercise due?</strong></summary>
    <p>Please submit your exercise within three (3) days of receiving it. Feel free to leave notes in <code>submission.md</code> to let us know what you would have done with more time — we'll appreciate the insight into your process!</p>
</details>
<br />
<details>
    <summary><strong>Do I have to setup a build tool (Gulp, WebPack, Grunt, etc.)?</strong></summary>
    <p>The build tool setup is part of the exercise, so we strongly encourage you to complete this step. If you absolutely can't set it up in time, skip that step and focus on the exercises in plain HTML/CSS/JS. When you submit your final assessment, please let us know why you skipped this build tool setup step in the <code>submission.md</code> file.</p>
</details>
<br />
<details>
    <summary><strong>What browsers should I support?</strong></summary>
    <p>We'll look for compatibility in the following browsers:</p>
    <ol>
        <li>Google Chrome (latest version)</li>
        <li>Mozilla Firefox (latest version)</li>
        <li>Microsoft Edge (latest version)</li>
    </ol>
</details>
<br />
<details>
    <summary><strong>What color values should I use?</strong></summary>
    <p>The exact color values don't matter; just match colors close enough to the mockup as they appear on your screen. You may use a Chrome extension such as <a href="https://chrome.google.com/webstore/detail/colorpick-eyedropper/ohcpnigalekghcmgcdcenkpelffpdolg?hl=en" target="_blank">ColorPick Eyedropper</a> or anything you're comfortable with to fetch the colors from the mockup.</p> 
</details>
<br />
<details>
    <summary><strong>I'm running out of time! May I skip one of the exercises?</strong></summary>
    <p>Although we expect you to finish all the exercises, life happens. If you aren't able to finish on time, focus on <code>Exercise 1 - Filterable Content</code> and start on the other exercise. Then give us some insight as to what you would have done in the <code>submission.md</code> file.</p>
</details>
<br />
<details>
    <summary><strong>Should I make a separate page for each exercise?</strong></summary>
    <p>No thanks — we'd like to see all the exercises on one page. This single page should look as similar to the mockup as possible.</p>
</details>
<br />
<details>
    <summary><strong>The instructions say to style the modules to match the mockups "without adding or removing HTML elements", but I need to add filters to the dropdown in <em>Exercise 1 — Filterable Content</em>. What should I do?</strong></summary>
    <p>You may add the filters dynamically anywhere you see fit in the existing markup. As long as the outer/non-dynamic structure (i.e. the original HTML) doesn’t change, that’s fine. It’s meant to be a tricky styling exercise.</p>
</details>
<br />
<details>
    <summary><strong>The instructions mention that I can use ES6 and React or Vue components, but the project itself uses EJS files. Normally, I would just build the page with React components and style them to match the mockup, but the instructions also say not to add or remove any of the HTML in the partials. Can I use the HTML that is in the EJS files, but as React or Vue components?</strong></summary>
    <p>It's fine to use the HTML that’s in the EJS files — as long as the structure and HTML tags don’t change for each component, we’ll accept that. It’s meant to be a styling challenge, so maintaining the structure is essential. Just add a note for us in the <code>submission.md</code> file saying you didn’t use the EJS files themselves but, instead, maintained the original EJS markup in the React or Vue components.</p>
</details>
