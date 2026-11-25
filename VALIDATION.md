# Validation

- Rendered the four pages with a Liquid template engine and Markdown renderer for the included offline preview.
- Checked for unrendered Liquid, exactly one main heading per page, duplicate IDs, correct navigation selection, local page links, and homepage links to research/project section anchors.
- Repeated template and local link checks with both an empty base URL and a `/portfolio` base URL.
- Checked text and button color contrast against the supplied dark palette.
- No external font or JavaScript requests are needed for the design.

The preview uses Python Liquid and Markdown rendering. It is not a substitute for a production Jekyll build. Ruby/Jekyll was unavailable in this workspace, and a working browser executable could not be obtained, so a full Jekyll build, browser rendering, keyboard interaction, and mobile overflow checks remain unverified. Responsive CSS includes layouts for desktop, tablet, and narrow screens; inspect them in your browser before publishing.

The source has not been pushed to GitHub or published.
