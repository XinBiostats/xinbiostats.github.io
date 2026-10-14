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

.cv-note {
  font-size: 0.8em;
  color: #8c9196;
  margin: 0.5em 0 0;
}
</style>

<div class="cv-bar">
  <span class="cv-bar__note">Last updated September 2026 &middot; 5 pages</span>
  <a class="cv-btn" href="{{ '/files/cv.pdf' | relative_url }}" target="_blank" rel="noopener">Download PDF</a>
</div>

<div class="cv-viewer">
  <iframe src="{{ '/files/cv.pdf' | relative_url }}" title="Curriculum vitae of Xin Ma"></iframe>
</div>

<p class="cv-note">Nothing showing above? Some mobile browsers can&rsquo;t display PDFs inline &mdash; <a href="{{ '/files/cv.pdf' | relative_url }}" target="_blank" rel="noopener">open the CV directly</a>.</p>
