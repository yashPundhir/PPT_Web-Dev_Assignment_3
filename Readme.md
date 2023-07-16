# Core Modules Assignment 3 - CSS (Media Queries)

---

**Q1.** What is a Media Query in CSS, and what is its purpose?

**Ans1.** In CSS, a media query is a feature that allows you to apply specific styles to a web page based on certain conditions, such as the characteristics of the device or the viewport size. It enables you to create responsive designs that adapt to different screen sizes and devices.

The purpose of using media queries is to create styles that are tailored to different devices or conditions, ensuring optimal user experience across various screen sizes and orientations. By applying different styles based on the media query conditions, you can adjust the layout, typography, colors, and other visual aspects of your website or application.

---

**Q2.** How do you define a media query in CSS?

**Ans2.** To define a media query in CSS, you use the `@media` rule followed by one or more conditions enclosed in parentheses. Here's the general syntax:

```css
@media <media-condition> {
	/* CSS rules to apply when the media condition is true */
}
```

The `<media-condition>` part is where you specify the conditions that determine when the styles within the media query block should be applied. Media conditions consist of one or more media features and their corresponding values.

Here's an example of a media query that targets devices with a maximum width of 600 pixels:

```css
@media (max-width: 600px) {
	/* CSS rules to apply for devices with a maximum width of 600px */
}
```

In the example above, `(max-width: 600px)` is the media condition. It uses the `max-width` media feature, which represents the maximum width of the viewport, and sets the value to `600px`. The CSS rules within the media query block will be applied only when the viewport width is 600 pixels or less.

You can also combine multiple conditions using logical operators `(and, or, not)` to create more complex media queries. Here's an example of a media query that targets devices with a maximum width of 600 pixels in portrait orientation:

```css
@media (max-width: 600px) and (orientation: portrait) {
	/* CSS rules to apply for devices with a maximum width of 600px in portrait orientation */
}
```

---

**Q3.** Explain the concept of Breakpoints in Responsive Web Design and How They are used in Media Queries.

**Ans3.** In responsive web design, breakpoints are specific points or ranges of viewport widths where the layout of a web page is adjusted to accommodate different screen sizes. Breakpoints serve as markers where the design `"breaks"` or changes to adapt to the available space on various devices.

Media queries are used in conjunction with breakpoints to apply specific styles or adjust the layout of elements based on different viewport sizes. By defining breakpoints and using media queries, you can create a responsive design that provides an optimal user experience across a range of devices.

Here's how breakpoints and media queries work together:

**Determining breakpoints:** Breakpoints are typically determined by analyzing common screen sizes and considering the content and layout of your web page. For example, you might choose breakpoints to target small mobile devices, tablets, and desktop screens.

**Defining media queries:** Once you've determined your breakpoints, you can use media queries to apply specific styles at each breakpoint. Each media query consists of a condition that evaluates to true when the viewport matches the specified criteria.

**Applying styles at breakpoints:** Within each media query block, you define the CSS rules that should be applied when the corresponding condition is met. These rules typically involve adjusting the layout, positioning, typography, or other visual aspects of your web page.

Here's an example that demonstrates the use of breakpoints and media queries:

```css
/* Styles for mobile devices */
@media (max-width: 480px) {
	/* CSS rules for small mobile screens */
}

/* Styles for tablets */
@media (min-width: 481px) and (max-width: 768px) {
	/* CSS rules for tablets */
}

/* Styles for desktop screens */
@media (min-width: 769px) {
	/* CSS rules for desktop screens */
}
```

---

**Q4.** What is the purpose of using Media Queries for Print Media?

**Ans4.** The purpose of using media queries for print media includes:

**Adjusting layout:** Media queries for print media enable you to modify the layout of your web page when it is printed. This can involve removing unnecessary elements that are not suitable for print, rearranging content for better readability, or creating a simplified version of the page optimized for the printed format.

**Controlling typography:** Print media queries allow you to specify different font sizes, line heights, and other typographic properties to improve legibility when content is printed. You can adjust the font styles and sizes to ensure that the text is clear and easy to read on paper.

**Managing colors:** When content is printed, colors may appear differently compared to on-screen display. Media queries for print media enable you to define specific color adjustments, such as changing background colors to white or light shades and adjusting text colors to ensure optimal contrast for printed output.

**Hiding or showing elements:** Media queries for print media can be used to hide or show specific elements selectively when the page is printed. This allows you to control which parts of the web page are included in the print output. For example, you might choose to hide navigation menus, advertisements, or other elements that are not relevant or useful in a printed document.

---

**Q5.** What is the purpose of the `orientation` media feature?

**Ans5.** The orientation media feature in CSS allows you to target styles based on the orientation of the device's viewport. It helps you customize the layout and presentation of your web page depending on whether the device is in a portrait or landscape orientation.

The purpose of the orientation media feature is to provide a more tailored and optimized user experience based on how the user holds or views their device. By utilizing this feature, you can make specific adjustments to the design, layout, or content placement to enhance usability and readability.

Here are a few examples of how the orientation media feature can be useful:

**Responsive layout adjustments:** You can use the orientation media feature to modify the layout of your web page to accommodate the available screen space in portrait or landscape mode. For instance, you might choose to stack elements vertically in portrait mode and display them side-by-side in landscape mode.

**Image and media handling:** By targeting the orientation media feature, you can optimize the presentation of images or media elements based on the available space. For example, you could adjust the dimensions, alignment, or scaling of an image to ensure it fits appropriately in either portrait or landscape mode.

**Typography and readability:** Depending on the orientation, the width and height proportions of the viewport change. You can leverage the orientation media feature to adjust the typography, line lengths, or spacing to maintain readability and legibility of your content.

---

**Q6.** Imagine you are a web developer working for a creative agency that specializes in building visually appealing and interactive websites. The agency has recently received a client request to create a landing page similar to the design of the one-page website: [One Card Website](https://www.getonecard.app/). The client wants to showcase a video prominently on the page to engage visitors.

Your task is to create a simple webpage that replicates the one-page landing page design, including a responsive layout and an HTML video. The below images are for your reference. Some browsers don’t allow you to play videos without the controls attribute. So, you can add controls here, we will learn how to play a video without the controls attribute in the later sections.

For Large Screen:

![img](https://pwskills.notion.site/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F529878ec-dfdf-4ea9-9198-0eb71b182bec%2F1.png?id=7ed23343-1e3b-4655-bc3a-cc5c1a90d982&table=block&spaceId=6fae2e0f-dedc-48e9-bc59-af2654c78209&width=2000&userId=&cache=v2)

For Small Screen:

![img](https://pwskills.notion.site/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F0472f14c-c72f-4a13-a43b-1bea11c78437%2F2.png?id=3c9cce86-5163-4439-9fd1-c7923a4d18ac&table=block&spaceId=6fae2e0f-dedc-48e9-bc59-af2654c78209&width=2000&userId=&cache=v2)

## [One Card Navbar & Hero Section](https://github.com/yashPundhir/One-Card-HomePage-UI)

---

**Q7.** You are tasked with building a webpage that displays an image gallery using a grid layout. The challenge is to ensure the gallery is visually appealing and functional on both large and small screens. On large screens, the gallery should display multiple images per row, while on small screens, it should collapse into a single column for optimal viewing. Refer to the attached images for visual reference. Implement this using CSS Grid and media queries for responsiveness.

![img](https://pwskills.notion.site/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fc0c9b12f-7ad7-4d43-8a1d-3a7296caa8c6%2F3.png?id=52fd127d-3e53-453c-990c-ed0691ab7125&table=block&spaceId=6fae2e0f-dedc-48e9-bc59-af2654c78209&width=2000&userId=&cache=v2)

![img](https://pwskills.notion.site/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F6b7d1874-feac-4be4-bd37-90122f54d024%2F4.png?id=4e744c0f-db2b-4e74-8934-0b7ef2152fa3&table=block&spaceId=6fae2e0f-dedc-48e9-bc59-af2654c78209&width=2000&userId=&cache=v2)

## [Grid Layout Code](https://github.com/yashPundhir/Grid_layout_UI)

---

**Q8.** In this coding challenge, your task is to create an information section for the previously built OneCard webpage clone, focusing on the different modes like dark and light modes. The webpage should look different depending on the screen size: dark mode for larger screens and light mode for smaller devices. The reference images are attached below.

![img](https://pwskills.notion.site/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F6aa9a291-1923-4caf-b34b-799c72b452f4%2F5.png?id=f17f069b-0f3e-41a6-a44e-1bc2e01ea7f7&table=block&spaceId=6fae2e0f-dedc-48e9-bc59-af2654c78209&width=2000&userId=&cache=v2)

![img](https://pwskills.notion.site/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F60b972ef-01de-49b3-bacc-21b6b98d4dd3%2F6.png?id=90159ed3-7d75-4146-adfa-75896ab86dbd&table=block&spaceId=6fae2e0f-dedc-48e9-bc59-af2654c78209&width=2000&userId=&cache=v2)

## [One Card Info Section](https://github.com/yashPundhir/One-Card-HomePage-UI)

---

**Q9.** You have reached the final task of learning responsive web design, which involves designing a responsive footer. Your goal is to build a simple webpage footer that matches the design shown in the attached image. The footer should adapt to different screen sizes, ensuring optimal visibility and alignment of the content. Refer to the attached image for a visual reference.

![img](https://pwskills.notion.site/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fdb124079-45bd-42ff-b782-5d1dc13ac288%2F7.png?id=dd69ae96-097d-4274-99d1-2f8703fad352&table=block&spaceId=6fae2e0f-dedc-48e9-bc59-af2654c78209&width=2000&userId=&cache=v2)

![img](https://pwskills.notion.site/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fa41975e1-ac00-4c06-bb1f-7436747dabf8%2F8.png?id=50ca5e75-3357-440c-8bf4-cf3ef68740f2&table=block&spaceId=6fae2e0f-dedc-48e9-bc59-af2654c78209&width=2000&userId=&cache=v2)

## [One Card Footer Section](https://github.com/yashPundhir/One-Card-HomePage-UI)

---

**Q10.** You have been given to create a student dashboard page that includes a student details table. The challenge lies in handling the table's display on different screen sizes. On large screens, the table should be fully visible, while on small screens, it should have an internal scroll to ensure proper visibility of information. Refer to the attached images for visual reference.

![img](https://pwskills.notion.site/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Ff99a5faa-be32-472f-b67f-e1a5bf3bc4a3%2F9.png?id=3de3b332-e76d-4145-a50e-b91bbe9dc766&table=block&spaceId=6fae2e0f-dedc-48e9-bc59-af2654c78209&width=2000&userId=&cache=v2)

![img](https://pwskills.notion.site/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fb545f6b0-5744-46a8-8418-ee29f1306fd6%2F10.png?id=63605578-84e4-4ede-a6c8-87336549f533&table=block&spaceId=6fae2e0f-dedc-48e9-bc59-af2654c78209&width=2000&userId=&cache=v2)

## [Student Dashboard Table Code](https://github.com/yashPundhir/Student_Dashboard_UI)

---
