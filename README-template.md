# Frontend Mentor - Results summary component solution

This is a solution to the [Results summary component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/results-summary-component-CE_K6s0maV). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page
- **Bonus**: Use the local JSON data to dynamically populate the content

### Screenshot

![](./screenshot.jpg)

Add a screenshot of your solution. The easiest way to do this is to use Firefox to view your project, right-click the page and select "Take a Screenshot". You can choose either a full-height screenshot or a cropped one based on how long the page is. If it's very long, it might be best to crop it.

Alternatively, you can use a tool like [FireShot](https://getfireshot.com/) to take the screenshot. FireShot has a free option, so you don't need to purchase it.

Then crop/optimize/edit your image however you like, add it to your project, and update the file path in the image above.

**Note: Delete this note and the paragraphs above when you add your screenshot. If you prefer not to add a screenshot, feel free to remove this entire section.**

### Links

- Solution URL: [Solution URL here](https://github.com/khabbab50/frontend-mentor-results-summary-component-main.git)
- Live Site URL: [Live site URL here](https://khabbab50.github.io/frontend-mentor-results-summary-component-main/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- [React](https://reactjs.org/) - JS library
- [Next.js](https://nextjs.org/) - React framework
- [Styled Components](https://styled-components.com/) - For styles

**Note: These are just examples. Delete this note and replace the list above with your own choices**

### What I learned

Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge.

To see how you can add code snippets, see below:

```html
<!-----------------------------------------------------------
      main section start
    ------------------------------------------------------------>
<main class="main">
  <!-- your result start  -->
  <div class="your-result">
    <h3>Your Result</h3>
    <div class="circl">
      <h1>76</h1>
      <p>of 100</p>
    </div>
    <h2>Great</h2>
    <p>You scored higher than 65% of the people who have taken these tests.</p>
  </div>
  <!-- your result end -->

  <!-- summary start  -->
  <div class="summary">
    <h3>Summary</h3>

    <div class="reaction flex-item">
      <p>
        <span><i class="fa-solid fa-bolt"></i> Reaction</span>
      </p>
      <p><strong>80</strong> / 100</p>
    </div>

    <div class="memory flex-item">
      <p>
        <span><i class="fa-brands fa-dribbble"></i> Memory</span>
      </p>
      <p><strong>92</strong> / 100</p>
    </div>

    <div class="verbal flex-item">
      <p>
        <span><i class="fa-regular fa-comment"></i> Verbal</span>
      </p>
      <p><strong>61</strong> / 100</p>
    </div>

    <div class="visual flex-item">
      <p>
        <span><i class="fa-regular fa-eye"></i> Visual</span>
      </p>
      <p><strong>72</strong> / 100</p>
    </div>

    <button class="btn">Continue</button>
  </div>
  <!-- summary end -->
</main>
<!-----------------------------------------------------------
      main section end
    ------------------------------------------------------------>
```

```css
/*============================================================
 main section  start  
 ===========================================================*/
body {
  height: 150vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.main {
  width: 700px;
  margin: 0 auto;
  display: flex;
  flex-wrap: wrap;
  box-shadow: 0.2rem 0.2rem 2rem hsl(221, 100%, 96%);
  border-radius: 30px;
}
/* your result start  */
.main .your-result {
  width: 50%;
  text-align: center;
  background: linear-gradient(
    to bottom,
    hsl(252, 100%, 67%),
    hsl(241, 81%, 54%)
  );
  padding: 50px;
  border-radius: 30px;
}
.main .your-result h3 {
  color: var(--light-lavender);
}
.main .your-result .circl {
  background: linear-gradient(
    to bottom,
    hsla(256, 72%, 46%, 1),
    hsla(241, 72%, 46%, 0)
  );
  width: 200px;
  height: 200px;
  margin: 30px auto;
  border-radius: 50%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  color: var(--white);
}
.main .your-result .circl h1 {
  font-size: 80px;
}
.main .your-result .circl p {
  color: hsl(241deg 100% 89% / 60%);
  font-size: 16px;
}
.main .your-result h2 {
  color: var(--white);
  margin-bottom: 20px;
  font-weight: 600;
  font-size: 30px;
}
.main .your-result p {
  color: var(--light-lavender);
}
/* your result end */

/* summary start  */
.main .summary {
  width: 50%;
  padding: 50px;
}
.main .summary h3 {
  margin-bottom: 20px;
  color: var(--dark-gray-blue);
  font-size: 25px;
}
.flex-item {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}
.main .summary .reaction {
  background: hsl(0deg 100% 67% / 10%);
  padding: 10px;
  border-radius: 8px;
  margin: 30px 0;
}
.main .summary .reaction p {
}
.main .summary .reaction span {
  color: var(--light-red);
}
.main .summary .memory {
  background: hsl(39deg 100% 56% / 10%);
  padding: 10px;
  border-radius: 8px;
  margin: 30px 0;
}
.main .summary .memory span {
  color: var(--orangey-yellow);
}
.main .summary .memory p {
}
.main .summary .verbal {
  background: hsl(166deg 100% 37% / 10%);
  padding: 10px;
  border-radius: 8px;
  margin: 30px 0;
}
.main .summary .verbal span {
  color: var(--reen-teal);
}
.main .summary .verbal p {
}
.main .summary .visual {
  background: hsl(234deg 85% 45% / 10%);
  padding: 10px;
  border-radius: 8px;
  margin: 30px 0;
}
.main .summary .visual span {
  color: var(--cobalt-blue);
}
.main .summary .visual p {
}
.main .summary .btn {
  width: 100%;
  padding: 20px 0;
  background: var(--dark-gray-blue);
  color: var(--white);
  border: none;
  border-radius: 30px;
  font-weight: 500;
  font-size: 18px;
  cursor: pointer;
}
.main .summary .btn:hover {
  background: linear-gradient(
    to bottom,
    hsl(252, 100%, 67%),
    hsl(241, 81%, 54%)
  );
}
/* summary end  */
/*============================================================
 main section end
 ===========================================================*/
```

```js
const proudOfThisFunc = () => {
  console.log("🎉");
};
```

If you want more help with writing markdown, we'd recommend checking out [The Markdown Guide](https://www.markdownguide.org/) to learn more.

**Note: Delete this note and the content within this section and replace with your own learnings.**

### Continued development

Use this section to outline areas that you want to continue focusing on in future projects. These could be concepts you're still not completely comfortable with or techniques you found useful that you want to refine and perfect.

**Note: Delete this note and the content within this section and replace with your own plans for continued development.**

### Useful resources

- [Example resource 1](https://www.example.com) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.
- [Example resource 2](https://www.example.com) - This is an amazing article which helped me finally understand XYZ. I'd recommend it to anyone still learning this concept.

**Note: Delete this note and replace the list above with resources that helped you during the challenge. These could come in handy for anyone viewing your solution or for yourself when you look back on this project in the future.**

## Author

- Website - [Md Khabbab Hossen](https://github.com/khabbab50)
- Frontend Mentor - [@khabbab50](https://www.frontendmentor.io/profile/khabbab50)
- Facebook - [@khabbab51](https://www.facebook.com/khabbab51)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**

## Acknowledgments

This is where you can give a hat tip to anyone who helped you out on this project. Perhaps you worked in a team or got some inspiration from someone else's solution. This is the perfect place to give them some credit.

**Note: Delete this note and edit this section's content as necessary. If you completed this challenge by yourself, feel free to delete this section entirely.**
