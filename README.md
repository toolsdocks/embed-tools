# toolsdocks: Free Tool Embed Codes for Your Website

Add useful online tools to your website with a small HTML snippet. Give visitors a file utility, an image tool, a calculator or a text tool without building it yourself.

**Get free hosted embed codes and view your tool stats at [business.toolsdocks.com](https://business.toolsdocks.com).**

[Choose a tool](https://business.toolsdocks.com) · [Browse all free tools](https://www.toolsdocks.com/tools) · [Installation steps](#how-to-add-a-free-tool-to-your-website) · [Embed code examples](#free-tool-embed-code-examples) · [View stats](#view-your-tool-stats-at-businesstoolsdockscom)

---

## How to add a free tool to your website

### 1. Choose your tool

Open **[business.toolsdocks.com](https://business.toolsdocks.com)**, follow the current account and website setup, and choose a compatible tool from the embed catalog.

You can try the public tools first at **[toolsdocks.com/tools](https://www.toolsdocks.com/tools)**.

### 2. Copy your embed code

Save your tool in the dashboard and copy its installation code. Each saved embed has its own **widget ID**.

A widget is simply the saved version of a tool that you add to your website.

### 3. Paste it and publish

Add an **HTML**, **Custom HTML** or **Embed** block where you want the tool to appear. Paste the complete code, then publish the page.

Open your published page on desktop and mobile to check the tool.

**No repository download, package installation or API key is needed to install a hosted embed.** Your website must allow the required script or iframe code.

> The snippets below are templates. Replace each `YOUR_..._WIDGET_ID` with the real ID of a tool saved in your dashboard. If your dashboard provides a different supported snippet, use that generated code.

---

## The simplest embed code

This format works with a saved toolsdocks hosted widget:

```html
<div data-toolsdocks-widget="YOUR_SAVED_WIDGET_ID"></div>
<script async src="https://www.toolsdocks.com/embed/v1.js"></script>
```

**Where does the ID come from?** Copy it from the installation code for your saved tool at **[business.toolsdocks.com](https://business.toolsdocks.com)**. A public tool URL or tool name is not a widget ID.

**Where do I paste the code?** Inside the website page's HTML or Embed block, where the tool should appear. Paste both lines together.

**Can I use more than one tool?** Yes. Add one widget container for each saved tool. When using the same page, include the loader script once after the containers.

```html
<div
  data-toolsdocks-widget="YOUR_FIRST_WIDGET_ID"
  data-title="First embedded tool"
></div>

<div
  data-toolsdocks-widget="YOUR_SECOND_WIDGET_ID"
  data-title="Second embedded tool"
></div>

<script async src="https://www.toolsdocks.com/embed/v1.js"></script>
```

The loader creates the tool's iframe and adjusts its height through the supported runtime. The saved widget controls its actual tool and settings.

---

## Free tool embed code examples

Use these examples after saving the corresponding compatible tool in the Business dashboard. The `data-title` attribute gives the iframe an accessible title; it does not select a different tool or change your account permissions.

### Batch file renamer

Give visitors a way to prepare filenames with patterns and numbering.

[Try the public Batch File Renamer](https://www.toolsdocks.com/tools/batch-file-renamer) · [Create a hosted embed](https://business.toolsdocks.com)

```html
<div
  data-toolsdocks-widget="YOUR_FILE_RENAMER_WIDGET_ID"
  data-title="Batch file renamer"
></div>
<script async src="https://www.toolsdocks.com/embed/v1.js"></script>
```

### Image format converter

Add an image conversion tool to a photography, design or ecommerce workflow.

[Try the public Image Format Converter](https://www.toolsdocks.com/tools/image-converter) · [Create a hosted embed](https://business.toolsdocks.com)

```html
<div
  data-toolsdocks-widget="YOUR_IMAGE_CONVERTER_WIDGET_ID"
  data-title="Image format converter"
></div>
<script async src="https://www.toolsdocks.com/embed/v1.js"></script>
```

### PDF merger and splitter

Help visitors work with PDF documents directly on a relevant page.

[Try the public PDF Merger and Splitter](https://www.toolsdocks.com/tools/pdf-merge-split) · [Create a hosted embed](https://business.toolsdocks.com)

```html
<div
  data-toolsdocks-widget="YOUR_PDF_WIDGET_ID"
  data-title="PDF merger and splitter"
></div>
<script async src="https://www.toolsdocks.com/embed/v1.js"></script>
```

### Word and character counter

A practical addition to writing resources, learning pages and content workflows.

[Try the public Word Counter](https://www.toolsdocks.com/tools/word-counter) · [Create a hosted embed](https://business.toolsdocks.com)

```html
<div
  data-toolsdocks-widget="YOUR_WORD_COUNTER_WIDGET_ID"
  data-title="Word and character counter"
></div>
<script async src="https://www.toolsdocks.com/embed/v1.js"></script>
```

### UTM link builder

Give marketers a convenient way to prepare campaign links.

[Try the public UTM Link Builder](https://www.toolsdocks.com/tools/utm-builder) · [Create a hosted embed](https://business.toolsdocks.com)

```html
<div
  data-toolsdocks-widget="YOUR_UTM_BUILDER_WIDGET_ID"
  data-title="UTM link builder"
></div>
<script async src="https://www.toolsdocks.com/embed/v1.js"></script>
```

### Add an accessible title to any saved tool

The same installation pattern applies to other compatible tools. Copy the correct widget ID from your dashboard and choose a descriptive title.

```html
<div
  data-toolsdocks-widget="YOUR_SAVED_WIDGET_ID"
  data-title="Describe the tool visitors will use"
></div>
<script async src="https://www.toolsdocks.com/embed/v1.js"></script>
```

---

## Iframe embed code

If your website accepts iframes but filters scripts, use the iframe option generated by the dashboard. The hosted loader inspected for this guide uses the `/embed/widget/` route shown below.

```html
<iframe
  src="https://www.toolsdocks.com/embed/widget/YOUR_SAVED_WIDGET_ID"
  title="Embedded website tool"
  width="100%"
  height="650"
  style="display:block;max-width:100%;border:0;"
  loading="lazy"
  allow="clipboard-write"
  sandbox="allow-scripts allow-same-origin allow-forms allow-downloads"
  referrerpolicy="strict-origin-when-cross-origin"
></iframe>
```

A plain iframe uses the height you set. It does not automatically resize to cross-origin content without cooperating host code. Increase its height if the tool is cut off.

Some website builders add their own iframe or sandbox around your code. Use the dashboard's tested platform instructions when a nested-frame installation needs a different supported snippet. If a tool or approved advertising format requires additional permissions, use the provider-generated iframe configuration rather than adding unrestricted permissions yourself.

---

## Install on your website builder

| Website builder | Where to put the code | Finish by |
| --- | --- | --- |
| **WordPress** | A **Custom HTML** block, if your account and site permit the script | Updating or publishing the page |
| **Elementor** | An **HTML** widget | Updating the page and opening its published URL |
| **GoHighLevel** | The current funnel or website builder's **Custom HTML / code** element | Saving and publishing the page |
| **Webflow** | A **Code Embed** element, when available on your plan | Publishing or using a supported preview |
| **Wix** | An **Embed HTML** or supported website-URL element | Setting a usable container height and publishing |
| **Shopify** | A supported **Custom Liquid** section or compatible theme code block | Saving the theme/page change |
| **Squarespace** | A supported **Code** block with the required permissions | Saving and checking the published page |
| **HTML website** | Inside the page's `<body>`, where you want the tool | Saving and publishing the HTML file |

**A builder name in this table does not guarantee every plan or editor accepts custom code.** If a script is stripped, use an allowed iframe or follow that platform's current supported instructions. A visible inline tool should go into a page content block, not an unrelated tracking-code field.

### WordPress example

1. Edit the page and add a **Custom HTML** block.
2. Paste the complete embed snippet.
3. Click **Update** or **Publish**, then open the public page.

### Elementor example

1. Open the page with Elementor and add an **HTML** widget.
2. Paste the complete embed snippet.
3. Update the page and check the public URL.

### GoHighLevel example

1. Open your funnel or website page in the builder.
2. Add the available custom HTML/code element and paste the snippet.
3. Save, publish and test the public page. Preview and published-page behavior can differ.

---

## View your tool stats at business.toolsdocks.com

**Open [business.toolsdocks.com](https://business.toolsdocks.com) to manage your hosted tools and view the usage information available in your dashboard.**

Your saved widget connects its hosted usage to the correct website and account. Available reporting depends on the current dashboard and account features.

- A **widget view** measures recorded widget loading, not every visit to your whole website.
- A **successful use** measures a completed tool operation under the service's usage rules.
- Clicking **Copy code** does not mean a tool is installed.
- This README and GitHub's repository views do not create tool-use statistics.
- Unregistered iframes or self-hosted copies do not automatically report usage to the Business dashboard.

Free hosted embeds follow the service's current usage allowance and may include advertising. Check the dashboard for the current free-use conditions. The public tools and the hosted embed service have separate usage behavior.

---

## More free tools to explore

| Tool | Useful for |
| --- | --- |
| [Batch Image Resizer](https://www.toolsdocks.com/tools/image-resizer) | Preparing multiple images |
| [JSON Formatter and Validator](https://www.toolsdocks.com/tools/json-formatter) | Inspecting and formatting JSON |
| [CSV Merger and Splitter](https://www.toolsdocks.com/tools/csv-merge-split) | Working with data exports |
| [Spreadsheet Comparison](https://www.toolsdocks.com/tools/spreadsheet-compare) | Finding differences between datasets |
| [Pivot Table Builder](https://www.toolsdocks.com/tools/pivot-table) | Summarizing spreadsheet data |
| [Invoice Generator](https://www.toolsdocks.com/tools/invoice-generator) | Preparing an invoice |
| [Email Signature Generator](https://www.toolsdocks.com/tools/email-signature) | Preparing an email signature |
| [QR Code Generator and Reader](https://www.toolsdocks.com/tools/qr-code) | Creating or reading QR codes |
| [Scientific Calculator](https://www.toolsdocks.com/tools/scientific-calculator) | Everyday mathematical calculations |
| [Pomodoro Focus Timer](https://www.toolsdocks.com/tools/pomodoro-timer) | Focus sessions and breaks |

Public tool links help you try the tools. **For installation, select an actually compatible hosted embed inside [business.toolsdocks.com](https://business.toolsdocks.com).** This README does not claim every public tool is currently embeddable.

<details>
<summary><strong>Browse the complete public catalog: 167 tool links</strong></summary>

Public catalog checked on 12 October 2026. Hosted embed compatibility is listed separately in the Business dashboard.

1. [Device-to-device file sharing](https://www.toolsdocks.com/tools/local-file-sharing)
2. [Shared clipboard between devices](https://www.toolsdocks.com/tools/shared-clipboard)
3. [Batch file renamer](https://www.toolsdocks.com/tools/batch-file-renamer)
4. [ZIP creator and extractor](https://www.toolsdocks.com/tools/zip-creator-extractor)
5. [Large-file splitter and rejoiner](https://www.toolsdocks.com/tools/file-splitter-joiner)
6. [Duplicate file finder](https://www.toolsdocks.com/tools/duplicate-file-finder)
7. [Folder comparison](https://www.toolsdocks.com/tools/folder-compare)
8. [File checksum verifier](https://www.toolsdocks.com/tools/checksum-verifier)
9. [Folder size analyzer](https://www.toolsdocks.com/tools/folder-size-analyzer)
10. [PDF merger and splitter](https://www.toolsdocks.com/tools/pdf-merge-split)
11. [PDF page organizer](https://www.toolsdocks.com/tools/pdf-page-organizer)
12. [PDF compressor](https://www.toolsdocks.com/tools/pdf-compressor)
13. [PDF annotation and signature](https://www.toolsdocks.com/tools/pdf-annotate-sign)
14. [PDF form filler](https://www.toolsdocks.com/tools/pdf-form-filler)
15. [Scanned document OCR](https://www.toolsdocks.com/tools/ocr)
16. [PDF text extractor](https://www.toolsdocks.com/tools/pdf-text-extractor)
17. [Office document to PDF](https://www.toolsdocks.com/tools/office-to-pdf)
18. [PDF to editable Word](https://www.toolsdocks.com/tools/pdf-to-word)
19. [Resume builder](https://www.toolsdocks.com/tools/resume-builder)
20. [Image format converter](https://www.toolsdocks.com/tools/image-converter)
21. [Target-size image compressor](https://www.toolsdocks.com/tools/image-compressor)
22. [Batch image resizer](https://www.toolsdocks.com/tools/image-resizer)
23. [Photo editor](https://www.toolsdocks.com/tools/photo-editor)
24. [Background remover](https://www.toolsdocks.com/tools/background-remover)
25. [Photo collage maker](https://www.toolsdocks.com/tools/collage-maker)
26. [Meme maker](https://www.toolsdocks.com/tools/meme-maker)
27. [Screenshot stitcher](https://www.toolsdocks.com/tools/screenshot-stitcher)
28. [Image metadata viewer and remover](https://www.toolsdocks.com/tools/image-metadata)
29. [Product mockup generator](https://www.toolsdocks.com/tools/product-mockups)
30. [Browser video editor](https://www.toolsdocks.com/tools/video-editor)
31. [Video compressor](https://www.toolsdocks.com/tools/video-compressor)
32. [Video format converter](https://www.toolsdocks.com/tools/video-converter)
33. [Subtitle editor](https://www.toolsdocks.com/tools/subtitle-editor)
34. [Subtitle format converter](https://www.toolsdocks.com/tools/subtitle-converter)
35. [Automatic subtitle generator](https://www.toolsdocks.com/tools/auto-subtitles)
36. [Subtitle burner](https://www.toolsdocks.com/tools/subtitle-burner)
37. [Video to GIF](https://www.toolsdocks.com/tools/video-to-gif)
38. [Video contact sheet](https://www.toolsdocks.com/tools/video-contact-sheet)
39. [Screen and webcam recorder](https://www.toolsdocks.com/tools/screen-recorder)
40. [Audio editor](https://www.toolsdocks.com/tools/audio-editor)
41. [Audio format converter](https://www.toolsdocks.com/tools/audio-converter)
42. [Voice recorder](https://www.toolsdocks.com/tools/voice-recorder)
43. [Audio transcription](https://www.toolsdocks.com/tools/audio-transcription)
44. [Text-to-speech generator](https://www.toolsdocks.com/tools/text-to-speech)
45. [Background noise reducer](https://www.toolsdocks.com/tools/noise-reducer)
46. [Audio loudness normalizer](https://www.toolsdocks.com/tools/loudness-normalizer)
47. [Ringtone maker](https://www.toolsdocks.com/tools/ringtone-maker)
48. [Online metronome](https://www.toolsdocks.com/tools/metronome)
49. [Audio waveform and spectrogram viewer](https://www.toolsdocks.com/tools/waveform-spectrogram)
50. [Word and character counter](https://www.toolsdocks.com/tools/word-counter)
51. [Reading and speaking time calculator](https://www.toolsdocks.com/tools/reading-time)
52. [Text case converter](https://www.toolsdocks.com/tools/case-converter)
53. [Duplicate-line remover](https://www.toolsdocks.com/tools/duplicate-line-remover)
54. [List sorter and filter](https://www.toolsdocks.com/tools/list-sorter)
55. [Text cleaner](https://www.toolsdocks.com/tools/text-cleaner)
56. [Text comparison](https://www.toolsdocks.com/tools/text-compare)
57. [Bulk find and replace](https://www.toolsdocks.com/tools/find-replace)
58. [Markdown editor](https://www.toolsdocks.com/tools/markdown-editor)
59. [Teleprompter](https://www.toolsdocks.com/tools/teleprompter)
60. [CSV viewer and editor](https://www.toolsdocks.com/tools/csv-editor)
61. [Spreadsheet data cleaner](https://www.toolsdocks.com/tools/data-cleaner)
62. [CSV, Excel and JSON converter](https://www.toolsdocks.com/tools/csv-excel-json-converter)
63. [CSV merger and splitter](https://www.toolsdocks.com/tools/csv-merge-split)
64. [Spreadsheet comparison](https://www.toolsdocks.com/tools/spreadsheet-compare)
65. [Email and phone list formatter](https://www.toolsdocks.com/tools/contact-list-formatter)
66. [Date-column normalizer](https://www.toolsdocks.com/tools/date-normalizer)
67. [Pivot table builder](https://www.toolsdocks.com/tools/pivot-table)
68. [Chart maker](https://www.toolsdocks.com/tools/chart-maker)
69. [Synthetic test-data generator](https://www.toolsdocks.com/tools/test-data-generator)
70. [JSON formatter and validator](https://www.toolsdocks.com/tools/json-formatter)
71. [YAML and XML formatter and validator](https://www.toolsdocks.com/tools/yaml-xml-formatter)
72. [Encoding toolkit](https://www.toolsdocks.com/tools/encoder-decoder)
73. [Regular expression tester](https://www.toolsdocks.com/tools/regex-tester)
74. [Code formatter and minifier](https://www.toolsdocks.com/tools/code-formatter)
75. [UUID generator](https://www.toolsdocks.com/tools/uuid-generator)
76. [JWT decoder](https://www.toolsdocks.com/tools/jwt-decoder)
77. [Cron expression builder and explainer](https://www.toolsdocks.com/tools/cron-builder)
78. [Unix timestamp converter](https://www.toolsdocks.com/tools/timestamp-converter)
79. [SQL playground](https://www.toolsdocks.com/tools/sql-playground)
80. [Color palette generator](https://www.toolsdocks.com/tools/color-palette)
81. [Color contrast checker](https://www.toolsdocks.com/tools/contrast-checker)
82. [CSS gradient generator](https://www.toolsdocks.com/tools/css-gradient)
83. [CSS shadow generator](https://www.toolsdocks.com/tools/css-shadow)
84. [Flexbox and CSS Grid playground](https://www.toolsdocks.com/tools/flexbox-grid-playground)
85. [SVG editor and optimizer](https://www.toolsdocks.com/tools/svg-editor)
86. [Favicon generator](https://www.toolsdocks.com/tools/favicon-generator)
87. [Font pairing previewer](https://www.toolsdocks.com/tools/font-pairing)
88. [Responsive layout previewer](https://www.toolsdocks.com/tools/responsive-preview)
89. [HTML accessibility checker](https://www.toolsdocks.com/tools/accessibility-checker)
90. [Search-result preview](https://www.toolsdocks.com/tools/serp-preview)
91. [Single-page SEO checker](https://www.toolsdocks.com/tools/seo-checker)
92. [Broken-link checker](https://www.toolsdocks.com/tools/broken-link-checker)
93. [XML sitemap generator](https://www.toolsdocks.com/tools/sitemap-generator)
94. [Robots.txt builder and checker](https://www.toolsdocks.com/tools/robots-txt)
95. [Structured-data generator](https://www.toolsdocks.com/tools/structured-data)
96. [Social-sharing preview checker](https://www.toolsdocks.com/tools/social-preview)
97. [Canonical and hreflang checker](https://www.toolsdocks.com/tools/hreflang-checker)
98. [UTM link builder](https://www.toolsdocks.com/tools/utm-builder)
99. [ROAS calculator](https://www.toolsdocks.com/tools/roas-calculator)
100. [Advertising metrics calculator](https://www.toolsdocks.com/tools/ad-metrics-calculator)
101. [Break-even ROAS calculator](https://www.toolsdocks.com/tools/break-even-roas)
102. [Sales funnel forecast](https://www.toolsdocks.com/tools/sales-funnel-forecast)
103. [Invoice generator](https://www.toolsdocks.com/tools/invoice-generator)
104. [Quote and estimate builder](https://www.toolsdocks.com/tools/quote-builder)
105. [Email signature generator](https://www.toolsdocks.com/tools/email-signature)
106. [WhatsApp link generator](https://www.toolsdocks.com/tools/whatsapp-link)
107. [Ecommerce order-profit calculator](https://www.toolsdocks.com/tools/order-profit-calculator)
108. [Loan payment and amortization calculator](https://www.toolsdocks.com/tools/loan-calculator)
109. [Compound interest calculator](https://www.toolsdocks.com/tools/compound-interest)
110. [Profit margin and markup calculator](https://www.toolsdocks.com/tools/margin-markup)
111. [Business break-even calculator](https://www.toolsdocks.com/tools/break-even-calculator)
112. [Savings goal calculator](https://www.toolsdocks.com/tools/savings-goal)
113. [Personal budget planner](https://www.toolsdocks.com/tools/budget-planner)
114. [Group expense splitter](https://www.toolsdocks.com/tools/expense-splitter)
115. [Tip, discount and sales-tax calculator](https://www.toolsdocks.com/tools/tip-tax-discount)
116. [Freelance hourly-rate calculator](https://www.toolsdocks.com/tools/freelance-rate)
117. [Subscription spending tracker](https://www.toolsdocks.com/tools/subscription-tracker)
118. [Time-zone converter and meeting planner](https://www.toolsdocks.com/tools/time-zone-planner)
119. [Meeting availability poll](https://www.toolsdocks.com/tools/meeting-poll)
120. [Date and working-day calculator](https://www.toolsdocks.com/tools/date-calculator)
121. [Pomodoro focus timer](https://www.toolsdocks.com/tools/pomodoro-timer)
122. [Work time tracker](https://www.toolsdocks.com/tools/time-tracker)
123. [Habit tracker](https://www.toolsdocks.com/tools/habit-tracker)
124. [To-do list and Kanban board](https://www.toolsdocks.com/tools/kanban-board)
125. [Shareable countdown timer](https://www.toolsdocks.com/tools/countdown-timer)
126. [Calendar event generator](https://www.toolsdocks.com/tools/ics-event-generator)
127. [Printable weekly planner](https://www.toolsdocks.com/tools/weekly-planner)
128. [Password and passphrase generator](https://www.toolsdocks.com/tools/password-generator)
129. [DNS record lookup](https://www.toolsdocks.com/tools/dns-lookup)
130. [SPF, DKIM and DMARC checker](https://www.toolsdocks.com/tools/email-auth-checker)
131. [IP subnet calculator](https://www.toolsdocks.com/tools/subnet-calculator)
132. [Microphone and webcam tester](https://www.toolsdocks.com/tools/mic-webcam-test)
133. [Keyboard tester](https://www.toolsdocks.com/tools/keyboard-tester)
134. [Mouse button and scroll tester](https://www.toolsdocks.com/tools/mouse-tester)
135. [Screen dead-pixel tester](https://www.toolsdocks.com/tools/dead-pixel-test)
136. [Browser capability checker](https://www.toolsdocks.com/tools/browser-capabilities)
137. [Internet speed test](https://www.toolsdocks.com/tools/speed-test)
138. [Scientific calculator](https://www.toolsdocks.com/tools/scientific-calculator)
139. [Percentage and ratio calculator](https://www.toolsdocks.com/tools/percentage-calculator)
140. [Fraction calculator](https://www.toolsdocks.com/tools/fraction-calculator)
141. [Function graphing tool](https://www.toolsdocks.com/tools/function-grapher)
142. [Equation and simultaneous-equation solver](https://www.toolsdocks.com/tools/equation-solver)
143. [Statistics calculator](https://www.toolsdocks.com/tools/statistics-calculator)
144. [Unit converter](https://www.toolsdocks.com/tools/unit-converter)
145. [GPA and grade calculator](https://www.toolsdocks.com/tools/gpa-calculator)
146. [Flashcard maker with practice mode](https://www.toolsdocks.com/tools/flashcards)
147. [Citation formatter](https://www.toolsdocks.com/tools/citation-formatter)
148. [Unit-price comparison](https://www.toolsdocks.com/tools/unit-price-compare)
149. [Recipe serving-size scaler](https://www.toolsdocks.com/tools/recipe-scaler)
150. [Paint quantity calculator](https://www.toolsdocks.com/tools/paint-calculator)
151. [Tile and flooring quantity calculator](https://www.toolsdocks.com/tools/tile-calculator)
152. [Travel packing-list builder](https://www.toolsdocks.com/tools/packing-list)
153. [Random name picker and spinning wheel](https://www.toolsdocks.com/tools/random-picker)
154. [Event seating-chart planner](https://www.toolsdocks.com/tools/seating-chart)
155. [Printable label maker](https://www.toolsdocks.com/tools/label-maker)
156. [Barcode generator](https://www.toolsdocks.com/tools/barcode-generator)
157. [QR code generator and reader](https://www.toolsdocks.com/tools/qr-code)
158. [Grammar and spelling assistant](https://www.toolsdocks.com/tools/grammar-checker)
159. [Paraphrasing and tone editor](https://www.toolsdocks.com/tools/paraphraser)
160. [Long-text summarizer](https://www.toolsdocks.com/tools/summarizer)
161. [Text translator](https://www.toolsdocks.com/tools/translator)
162. [Meeting transcript to notes and action items](https://www.toolsdocks.com/tools/meeting-notes)
163. [Plain-language explainer](https://www.toolsdocks.com/tools/plain-language)
164. [Blog and video outline generator](https://www.toolsdocks.com/tools/outline-generator)
165. [Image alt-text generator](https://www.toolsdocks.com/tools/alt-text-generator)
166. [Receipt data extractor](https://www.toolsdocks.com/tools/receipt-extractor)
167. [Document question answering](https://www.toolsdocks.com/tools/document-qa)

</details>

---

## Need a free game to embed?

These independent open-source game repositories are useful references if you want to host a browser game yourself. They are separate from the toolsdocks hosted-tool catalog.

| Repository | Game | License listed by the project |
| --- | --- | --- |
| [gabrielecirulli/2048](https://github.com/gabrielecirulli/2048) | Sliding number puzzle | MIT |
| [jakesgordon/javascript-tetris](https://github.com/jakesgordon/javascript-tetris) | JavaScript falling-block game | MIT |
| [Hextris/hextris](https://github.com/Hextris/hextris) | Hexagonal puzzle game | GPL-3.0-or-later |

For a self-hosted game, publish the project's playable HTML files on a host that permits embedding, then point an iframe at **your actual published game URL**:

```html
<iframe
  src="https://YOUR_GAME_HOST.example/game/"
  title="Your browser game"
  width="100%"
  height="650"
  style="display:block;max-width:100%;border:0;"
  loading="lazy"
></iframe>
```

Replace the example URL after publishing. A GitHub repository page or a `raw.githubusercontent.com` source file is not a playable iframe URL. Follow each project's license, preserve required notices, and check any separate asset licenses before redistributing it. Third-party demo availability and framing permissions can change.

---

## Common installation questions

### The code appears as text. What should I do?

Paste it into an **HTML** or **Embed** block, not a paragraph or rich-text block.

### The tool does not appear.

Check that the page is published, the widget ID belongs to a saved tool, and the website builder allows the selected code type. Open the published page rather than relying only on the editor preview.

### The tool is cut off on mobile.

Use responsive width. Increase an iframe or builder container's height when necessary. The supported script loader can resize the inner tool, but it cannot always resize a website builder's outer embed container.

### Can I embed the public toolsdocks page directly?

Use a saved hosted widget's generated code. A normal public tool page may have navigation, advertising or framing restrictions and is not the same as an embed runtime.

### Do visitors need a toolsdocks account?

The hosted embed is designed for visitors to use without signing into the owner's dashboard. The website owner manages the saved tool and installation through their account.

### Can this README track my website visitors?

No. It is documentation. For recorded hosted-tool usage, open **[business.toolsdocks.com](https://business.toolsdocks.com)**. The dashboard does not automatically measure every visit to the surrounding website.

### Where can I get help?

For tool installation and account-specific questions, use the support options available at **[business.toolsdocks.com](https://business.toolsdocks.com)**. For a correction to this guide, open an issue in the repository where this README is published. Never post account passwords, private files or secret keys.

---

## Contributing to this free embed-code guide

Useful contributions include clearer installation steps, verified compatible-tool examples, accessibility improvements and corrections to public tool links.

Before suggesting an embed:

- Test it on a published page with a real saved widget or self-hosted game URL.
- Explain which website builder and browser you tested.
- Do not publish private widget IDs or account data without permission.
- Do not add broken examples, bypass subscription checks or label an unlicensed project open source.

This repository is a documentation and snippet collection. It does not contain the toolsdocks hosted platform's source code. Independently linked game projects retain their own licenses.

## Project references

- [toolsdocks public tool catalog](https://www.toolsdocks.com/tools)
- [toolsdocks Business: hosted embeds and stats](https://business.toolsdocks.com)
- [GitHub's README guidance](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes)
- [Game-Embed-Codes: the simple README layout reference](https://github.com/USBHeadphones/Game-Embed-Codes)

The toolsdocks loader route and public tool links were checked on 12 October 2026. The code examples need your own saved widget ID; no account-specific hosted installation was created or tested for this document.

---

**Choose a free tool, copy its embed code and add it to your website.**

**[Get started and view your hosted-tool stats at business.toolsdocks.com →](https://business.toolsdocks.com)**

<!-- Maintainer setup, not extra files: Suggested repository name: toolsdocks-free-embed-codes. Suggested About description: Free embed codes for website tools, calculators, file utilities and browser games. Simple HTML installation guides from toolsdocks. Hosted-tool stats at business.toolsdocks.com. Suggested homepage: https://business.toolsdocks.com. Suggested topics: toolsdocks, embed-code, website-tools, free-tools, website-widgets, html, javascript, iframe, wordpress, elementor, gohighlevel, webflow, wix, shopify, calculators, text-tools, csv-tools, image-tools, browser-games, documentation. Add only relevant topics and replace this comment if the repository purpose changes. -->
