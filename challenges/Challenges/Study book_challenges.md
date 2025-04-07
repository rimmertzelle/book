# Study book - challenges

This year's challenge classes will focus on the correct use of HTML structural elements, mobile-first design with TailwindCSS, and utilizing an API with Asynchronous JavaScript (AJAX).

### Learning goals

- The student uses modern web techniques (HTML and Tailwind) to implement a design that functions correctly on all browsers and consumes data from an API.

### The final assignment

You will implement a design for a simple web application that utilizes web services through a RESTful API.

Steps to successfully finish this assignment

1. **Choose API and create a simple design**
- [ ]  Choose your own API (everyone needs to have a unique API)
- [ ]  Create a [design](Study%20book%20-%20challenges%200a95804b300a4a97acba61792ba5c1f8.md) (for example in Figma) you want to implement using your API
- [ ]  Hand in your design and API of choice

**Guidelines for the design.**

- Do not make it to complex
- Mobile first is important: however you need to design a dekstop variant as well.
- There is at least one details page that can be accessed via a click on the home page
- All pages have relevant data that comes from the API
- The design should be different than the design used in the classes and unique compared to other students
- For mobile and web: at least one overview and one details page

1. **Delivering the design**
- [ ]  Implement the design
- [ ]  Zip the project (use .zip and **not** .rar or another exotic extension)
- [ ]  Host the project (for example on render.com)
- [ ]  Hand in the link to the hosted solution and the zipped code on learn

### Grading

If you want your project to be graded, you have meet the next conditions

1. API and Design are approved
2. The original (approved) design is implemented
3. Code is handed in as a zipfile. (use .zip and **not** .rar or another exotic extension)
4. A working example of the code is available for testing purpose

**Rubric**

For each criteria you will be given 0 or all points.

| **Part** | **HTML** | **CSS layout** | **CSS mobile first** | **AJAX requests** | **Concurrent AJAX requests** |
| --- | --- | --- | --- | --- | --- |
| **Points (40)** | **8** | **4** | **4** | **20** | **4** |
| **Do’s** | Use of structural elements, like `<section>`, `<nav>` and `<aside>` | Use of `flexbox` and or `grid` for positioning | Use of the Tailwindcss mobile approach (e.g. add `sm:` etc before classes | Use `fetch` or `async` `await` for fetching data from an external web service | `Promise.all()` or an equivalent is used for handling concurrent requests |
| **Don’t** | I will pay attention to the amount of `<span>` and `<div>` that can be changed to other elements | I will pay attention to the amount of `<br/>`, `px` and or misuse of `padding` and `margin`. | Too many breakpoints are added | Not handling `errors` correctly | You didn’t implement concurrent requests |

### Classes

| Class | Topic |
| --- | --- |
| 1 | [AJAX and working with an API](Material%20dd713eee106c4d049e3dc61c48d0d4a8/JS%20-%20Asynchronous%20computing%206fcbd84868cf4605b6ea4c052fbc0b2f.md) |
| 2 | [Concurrent requests](Material%20dd713eee106c4d049e3dc61c48d0d4a8/JS%20-%20Asynchronous%20computing%206fcbd84868cf4605b6ea4c052fbc0b2f.md) and [Cors](Material%20dd713eee106c4d049e3dc61c48d0d4a8/Aside%20-%20Cors%2071b5eadfe9204810a4f6a915fc3019e5.md) |
| 3 | [HTML structural elements](Material%20dd713eee106c4d049e3dc61c48d0d4a8/HTML%20-%20structural%20element%2065188a568c1b473bb6155434e280a99e.md) |
| 4 | [CSS with Tailwind](Material%20dd713eee106c4d049e3dc61c48d0d4a8/CSS%20-%20tailwind%20and%20positioning%20cb2d50db95ee4bd69843d3e518ccc180.md) |