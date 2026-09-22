# YouTube Video Filter for Educators

An accessible, browser-based tool that helps educators find, evaluate, and embed instructional YouTube videos. The application converts a teaching need into a focused YouTube search, produces an AI-assisted research prompt, guides the educator through a verification checklist, and generates privacy-enhanced responsive embed code for Canvas or another learning platform.

## Live Application

**Launch the tool:** [https://eygarcia.github.io/youtube_video_filter/](https://eygarcia.github.io/youtube_video_filter/)

## Purpose

Finding a video is easy. Selecting a video that is accurate, accessible, age-appropriate, instructionally aligned, and safe for classroom use requires a deliberate review process.

This tool helps educators:

- Describe a learning objective and intended audience.
- Create a focused YouTube search query.
- Generate a detailed research prompt for an AI assistant.
- Evaluate candidate videos using a structured checklist.
- Confirm captions, credibility, accessibility, and classroom suitability.
- Create responsive YouTube embed code for Canvas.
- Use YouTube’s privacy-enhanced `youtube-nocookie.com` domain.

## Four-Step Workflow

### 1. Describe

Enter the instructional topic, subject, audience, learning objective, activity type, preferred duration, language, upload-date preference, and desired video qualities.

### 2. Search

The tool creates:

- A focused YouTube search query.
- A detailed AI research prompt requesting multiple recommendations and a comparison.
- Quick links for ChatGPT, Claude, NotebookLM, Gemini, and Microsoft Copilot.

AI recommendations must be verified by opening the live YouTube page. AI systems can return outdated titles, incorrect metadata, or nonexistent links.

### 3. Verify

Review the candidate video for:

- Instructional alignment
- Accuracy and currency
- Source credibility
- Bias and balanced representation
- Age appropriateness
- Caption quality and accessibility
- Advertising and distracting content
- Copyright considerations
- Embedding permissions
- Availability of a backup resource

### 4. Get Code

Generate and preview responsive iframe code that can be placed in:

- Canvas assignments, pages, discussions, or modules
- GitHub Pages
- Classroom websites
- Other systems that support iframe embedding

The generator supports privacy-enhanced mode, optional start time, player controls, fullscreen settings, accessible iframe titles, copy-to-clipboard, and print/save-to-PDF.

## Key Features

- One self-contained `index.html` file
- No server, database, build process, or API key required
- Responsive desktop, tablet, and mobile layout
- Keyboard-accessible navigation
- Visible focus indicators
- Screen-reader-friendly labels and status updates
- Reduced-motion support
- Local browser saving with `localStorage`
- Built-in help and classroom examples
- Search-prompt and embed-code copy buttons
- Privacy-enhanced YouTube embedding
- Canvas-oriented instructions and troubleshooting

## Technology

- HTML5
- Embedded CSS
- Vanilla JavaScript
- Browser `localStorage`
- YouTube and `youtube-nocookie.com` URLs

No third-party JavaScript libraries are required.

## Repository Structure

```text
youtube_video_filter/
├── index.html
└── README.md
```

## GitHub Pages Deployment

1. Place `index.html` and `README.md` in the repository root.
2. Open the repository’s **Settings**.
3. Select **Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select the `main` branch and `/ (root)` folder.
6. Select **Save**.
7. Allow GitHub Pages a few minutes to publish the application.

Expected address:

```text
https://eygarcia.github.io/youtube_video_filter/
```

## Canvas Integration

### Option 1: Add a Link

Add the live GitHub Pages address to a Canvas module, page, assignment, or discussion:

```text
https://eygarcia.github.io/youtube_video_filter/
```

### Option 2: Embed the Complete Tool

Open the Canvas HTML editor and add:

```html
<iframe
  src="https://eygarcia.github.io/youtube_video_filter/"
  title="YouTube Video Filter for Educators"
  width="100%"
  height="900"
  loading="lazy"
  style="border:1px solid #cccccc; border-radius:8px;"
  allowfullscreen>
</iframe>
```

After publishing, use **Student View** to test keyboard access, mobile layout, scrolling, and browser privacy restrictions.

Canvas administrators can restrict external iframe sources through institutional security settings.

## Privacy and Data Handling

- Form information is stored only in the user’s browser through `localStorage`.
- The application does not use a database or transmit form contents to a server.
- Selecting an AI platform opens that service in a new tab.
- The educator must paste the generated prompt into the selected AI service manually.
- Privacy-enhanced video embedding uses `youtube-nocookie.com`.
- Educators should still follow institutional privacy and student-data policies.
- Do not enter confidential student information into the tool or an AI prompt.

## Accessibility Review

Before assigning a video:

- Enable and inspect captions for accuracy.
- Provide a transcript or equivalent text resource when required.
- Confirm that essential information is not communicated only through sound, color, or rapidly changing visuals.
- Use a meaningful iframe title.
- Allow students to pause, replay, and control playback.
- Test the completed Canvas page with keyboard navigation.
- Test the published activity using Canvas Student View.
- Provide an alternative resource when required by an accommodation.

## Responsible AI Use

The generated AI prompt is intended to help locate and compare candidate videos. It does not independently verify that a recommended video exists or is appropriate.

Educators should:

- Open every recommended URL.
- Verify the exact title and channel.
- Confirm the publication date and runtime.
- Review the complete video.
- Inspect caption accuracy.
- Evaluate the source’s credibility.
- Check for bias, advertising, and age-inappropriate material.
- Confirm that embedding is permitted.
- Maintain a backup instructional resource.

## Troubleshooting

| Problem | Recommended action |
|---|---|
| GitHub Pages displays a 404 error | Confirm Pages is enabled for the `main` branch and `/ (root)` folder. |
| The page displays the wrong application | Confirm the YouTube Filter’s `index.html` is in this repository, not the main portfolio file. |
| A video will not play in Canvas | Confirm the creator permits embedding and provide the direct YouTube link as a backup. |
| YouTube results are too broad | Add the audience, learning objective, desired format, and important constraints. |
| An AI assistant provides a broken link | Open YouTube and independently verify the title, channel, URL, runtime, and publication date. |
| Changes do not appear immediately | Wait several minutes and perform a hard refresh with `Ctrl+F5`. |
| The page shows an older version | Clear the browser cache or open the site in a private browsing window. |
| Copy-to-clipboard does not work | Confirm that the browser permits clipboard access, or manually select and copy the generated text. |
| The generated iframe disappears in Canvas | Paste it through the Canvas HTML editor and confirm institutional iframe restrictions. |

## Updating the Application

The application is contained in one file:

```text
index.html
```

To publish an updated version:

1. Open the repository.
2. Select `index.html`.
3. Select the pencil-shaped **Edit** button.
4. Replace or update the code.
5. Select **Commit changes**.
6. Allow GitHub Pages several minutes to rebuild the site.
7. Refresh the published application using `Ctrl+F5`.

Do not replace `index.html` with the main GitHub portfolio page. The portfolio should be stored separately in the `eygarcia.github.io` repository.

## Educational Use

This project is designed for instructional use by educators and students. Always review third-party videos for:

- Accuracy
- Accessibility
- Copyright
- Privacy
- Advertising
- Source credibility
- Bias
- Age appropriateness
- Alignment with the course learning objective

YouTube content can be removed, renamed, edited, restricted, or made private without notice. Maintain a backup resource for important lessons.

## Author

**Edmond Garcia**  
Computer Network Systems Engineering and Cybersecurity  
Moorpark College

GitHub: [https://github.com/eygarcia](https://github.com/eygarcia)
