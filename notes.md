Here is the summary of your technical challenges and solutions translated into English. This structure follows the logic of a real-world development project.

---

## Project Technical Summary

### Phase 1: Architecture and Variables (CSS :root)
**Question:** How can I manage colors and fonts so the code is easy to maintain?
**Answer:** We used **Custom Properties** (CSS variables) within the `:root` selector. This allows defining values once (e.g., `--slate-300`) and reusing them everywhere. If a client asks to change blue to green, you only modify it in one place.

### Phase 2: Layout and Centering (Flexbox)
**Question:** How do I place the card exactly in the center of the browser?
**Answer:** We transformed the `body` into a **Flexbox** container. By using `justify-content: center` (main axis) and `align-items: center` (cross axis) with a `min-height` of `100vh`, the card remains centered regardless of screen size.

### Phase 3: Layout Debugging and Screenshots
**Question:** Why did the card appear shifted to the left in the screenshot even though it looked centered in the browser?
**Answer:** The issue was the use of `position: absolute` combined with `width: 100%` on the footer. This forced the browser to calculate an invisible width that "pushed" the card off-center during image generation. We solved this by using `flex-direction: column`, which stacks the card and footer naturally and cleanly.

### Phase 4: Images and Paths
**Question:** Why do images or styles sometimes fail to load online on GitHub?
**Answer:** Online paths are **case-sensitive** and require precision. We learned to use relative paths (e.g., `./screenshot.png`) and to verify that file names in the code match the folder names exactly.

### Phase 5: Documentation and Deployment (GitHub)
**Question:** How do I show my work live and document it professionally?
**Answer:** We created a `README.md` file using Markdown syntax to include screenshots and links. Finally, we activated **GitHub Pages**, which provides free hosting, turning your `index.html` and `style.css` files into a public website accessible via URL.

### Phase 6: The Final Touch (Accessibility and Credits)
**Question:** How can I correctly link my work to my professional profile?
**Answer:** We inserted dynamic links to your **Frontend Mentor** profile in both the HTML footer and the README. This ensures that anyone viewing the project knows it was built by you (Marcello Betti).

---