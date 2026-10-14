---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
---

<style>
.cv-bar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 0.6em;
  border-bottom: 1px solid #e6e8ea;
  padding-bottom: 0.6em;
  margin: 0.3em 0 1em;
}
.cv-bar__note {
  font-size: 0.82em;
  color: #8c9196;
}
.cv-btn {
  display: inline-block;
  padding: 0.45em 0.95em;
  border: 1px solid #52adc8;
  border-radius: 4px;
  background: #52adc8;
  color: #fff !important;
  font-size: 0.85em;
  font-weight: 600;
  text-decoration: none !important;
  white-space: nowrap;
  transition: background 0.15s ease, border-color 0.15s ease;
}
.cv-btn:hover, .cv-btn:focus {
  background: #3d8299;
  border-color: #3d8299;
  color: #fff !important;
  text-decoration: none !important;
}

.cv-viewer {
  width: 100%;
  aspect-ratio: 612 / 792;   /* US Letter, so a full page fits without cropping */
  max-height: 88vh;          /* but never taller than the window */
  min-height: 420px;
  border: 1px solid #e6e8ea;
  border-radius: 6px;
  overflow: hidden;
  background: #f4f6f7;
}
.cv-viewer object,
.cv-viewer iframe { display: block; width: 100%; height: 100%; border: 0; }

/* shown only when the browser cannot display the PDF inline */
.cv-fallback {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100%;
  padding: 2em 1.5em;
  text-align: center;
  color: #6b7177;
  font-size: 0.9em;
  line-height: 1.6;
}
.cv-fallback .cv-btn { margin-top: 0.9em; }
</style>

<div class="cv-bar">
  <span class="cv-bar__note">Last updated September 2026 &middot; 5 pages</span>
  <a class="cv-btn" href="{{ '/files/cv.pdf' | relative_url }}" target="_blank" rel="noopener">Download PDF</a>
</div>

<div class="cv-viewer">
  <object data="{{ '/files/cv.pdf' | relative_url }}" type="application/pdf" aria-label="Curriculum vitae of Xin Ma">
    <div class="cv-fallback">
      <div>Your browser can&rsquo;t display PDFs inline &mdash; this is common on mobile.</div>
      <a class="cv-btn" href="{{ '/files/cv.pdf' | relative_url }}" target="_blank" rel="noopener">Open CV (PDF)</a>
    </div>
  </object>
</div>
