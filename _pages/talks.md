---
layout: archive
title: "Talks and Presentations"
permalink: /talks/
author_profile: true
---

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/leaflet/1.9.4/leaflet.min.css" crossorigin="anonymous" referrerpolicy="no-referrer">

<style>
.talk-h {
  font-size: 1.1em;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: #6b7177;
  border-bottom: 1px solid #e6e8ea;
  padding-bottom: 0.4em;
  margin: 2.2em 0 1.1em;
}
.talk-h:first-of-type { margin-top: 0.5em; }

/* ---- map ---- */
#talkmap {
  height: 430px;
  border: 1px solid #e6e8ea;
  border-radius: 6px;
  margin: 0.3em 0 0.6em;
  background: #f4f6f7;
  z-index: 0;
}
@media (max-width: 37.5em) { #talkmap { height: 320px; } }

.talkmap-hint {
  font-size: 0.78em;
  color: #8c9196;
  margin: 0 0 0.4em;
}

.leaflet-tooltip.talk-tip {
  max-width: 300px;
  white-space: normal;
  padding: 0.6em 0.75em;
  border: 1px solid #dfe2e4;
  border-radius: 5px;
  box-shadow: 0 4px 14px rgba(30, 40, 50, 0.16);
  font-size: 0.8rem;
  line-height: 1.45;
  color: #4a4f54;
}
.talk-tip__place {
  font-weight: 700;
  color: #3b4045;
  margin-bottom: 0.35em;
}
.talk-tip__item + .talk-tip__item {
  margin-top: 0.55em;
  padding-top: 0.55em;
  border-top: 1px solid #eceef0;
}
.talk-tip__meta {
  font-size: 0.92em;
  color: #52adc8;
  font-weight: 600;
}
.talk-tip__topic { font-style: italic; }
.talk-tip__award { color: #b07d2b; font-size: 0.92em; }

/* ---- list ---- */
.talk-list { list-style: none; padding: 0; margin: 0; }
.talk-list li {
  padding: 0 0 0.9em;
  margin-bottom: 0.9em;
  border-bottom: 1px solid #f0f2f3;
  line-height: 1.5;
}
.talk-list li:last-child { border-bottom: 0; }
.talk-list .talk-meta {
  font-size: 0.8em;
  letter-spacing: 0.03em;
  text-transform: uppercase;
  color: #8c9196;
  margin-bottom: 0.15em;
}
.talk-list .talk-topic { color: #3b4045; }
.talk-list .talk-award {
  display: inline-block;
  margin-top: 0.3em;
  font-size: 0.82em;
  color: #b07d2b;
}
</style>

<h2 class="talk-h">Where I've Presented</h2>

<div id="talkmap"></div>
<p class="talkmap-hint">Hover over a marker for details (tap on mobile). Scroll to zoom after clicking the map.</p>

<h2 class="talk-h">Oral Presentations</h2>

<ul class="talk-list">
  <li>
    <div class="talk-meta">March 2026 &middot; ENAR Spring Meeting &middot; Indianapolis, IN</div>
    <div class="talk-topic">Reference-Informed Spatial Domain Detection Using Weak Supervision for Spatial Transcriptomics</div>
    <span class="talk-award">Session chair, &ldquo;Machine Learning and Causal Inference for Clinical and Genomic Studies&rdquo; &middot; Department PhD Student Travel Award</span>
  </li>
  <li>
    <div class="talk-meta">April 2024 &middot; PHHP Research Days &middot; Gainesville, FL</div>
    <div class="talk-topic">Deep5hmC: Predicting genome-wide 5-Hydroxymethylcytosine (5hmC) landscape via multimodal deep learning model</div>
  </li>
  <li>
    <div class="talk-meta">March 2024 &middot; Annual ASA Florida Chapter Meeting &middot; Tallahassee, FL</div>
    <div class="talk-topic">Deep5hmC: Predicting genome-wide 5-Hydroxymethylcytosine (5hmC) landscape via multimodal deep learning model</div>
  </li>
  <li>
    <div class="talk-meta">October 2023 &middot; Mark C. K. Yang Event &middot; Gainesville, FL</div>
    <div class="talk-topic">Deep5hmC: Predicting genome-wide 5-Hydroxymethylcytosine (5hmC) landscape via multimodal deep learning model</div>
    <span class="talk-award">Mark C. K. Yang Student Presentation Award</span>
  </li>
  <li>
    <div class="talk-meta">July 2023 &middot; ICIBM &middot; Tampa, FL</div>
    <div class="talk-topic">Integrated Spatial Multi-omics Analysis Based on MALDI Data</div>
  </li>
</ul>

<h2 class="talk-h">Poster Presentations</h2>

<ul class="talk-list">
  <li>
    <div class="talk-meta">March 2025 &middot; ENAR &middot; New Orleans, LA</div>
    <div class="talk-topic">SemiGraphST: A Semi-Supervised Deep Learning Approach for Domain Detection in Spatial Transcriptomics</div>
  </li>
  <li>
    <div class="talk-meta">March 2024 &middot; MCBIOS &middot; Atlanta, GA</div>
    <div class="talk-topic">Deep5hmC: Predicting genome-wide 5-Hydroxymethylcytosine (5hmC) landscape via multimodal deep learning model</div>
    <span class="talk-award">MCBIOS 2024 Travel Fellowship</span>
  </li>
  <li>
    <div class="talk-meta">November 2023 &middot; Florida Genetics Symposium &middot; Gainesville, FL</div>
    <div class="talk-topic">Deep5hmC: Predicting genome-wide 5-Hydroxymethylcytosine (5hmC) landscape via multimodal deep learning model</div>
  </li>
</ul>

<script src="https://cdnjs.cloudflare.com/ajax/libs/leaflet/1.9.4/leaflet.min.js" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
<script>
(function () {
  var el = document.getElementById('talkmap');
  if (!el || typeof L === 'undefined') return;

  // One entry per city; talks[] lists everything presented there.
  var PLACES = [
    {
      place: 'Indianapolis, IN',
      lat: 39.7684, lng: -86.1581,
      talks: [
        { date: 'March 2026', venue: 'ENAR Spring Meeting', kind: 'Oral',
          topic: 'Reference-Informed Spatial Domain Detection Using Weak Supervision for Spatial Transcriptomics',
          award: 'Department PhD Student Travel Award' }
      ]
    },
    {
      place: 'New Orleans, LA',
      lat: 29.9511, lng: -90.0715,
      talks: [
        { date: 'March 2025', venue: 'ENAR', kind: 'Poster',
          topic: 'SemiGraphST: A Semi-Supervised Deep Learning Approach for Domain Detection in Spatial Transcriptomics' }
      ]
    },
    {
      place: 'Gainesville, FL',
      lat: 29.6516, lng: -82.3248,
      talks: [
        { date: 'April 2024', venue: 'PHHP Research Days', kind: 'Oral',
          topic: 'Deep5hmC: Predicting genome-wide 5hmC landscape via multimodal deep learning model' },
        { date: 'November 2023', venue: 'Florida Genetics Symposium', kind: 'Poster',
          topic: 'Deep5hmC: Predicting genome-wide 5hmC landscape via multimodal deep learning model' },
        { date: 'October 2023', venue: 'Mark C. K. Yang Event', kind: 'Oral',
          topic: 'Deep5hmC: Predicting genome-wide 5hmC landscape via multimodal deep learning model',
          award: 'Mark C. K. Yang Student Presentation Award' }
      ]
    },
    {
      place: 'Tallahassee, FL',
      lat: 30.4383, lng: -84.2807,
      talks: [
        { date: 'March 2024', venue: 'Annual ASA Florida Chapter Meeting', kind: 'Oral',
          topic: 'Deep5hmC: Predicting genome-wide 5hmC landscape via multimodal deep learning model' }
      ]
    },
    {
      place: 'Atlanta, GA',
      lat: 33.7490, lng: -84.3880,
      talks: [
        { date: 'March 2024', venue: 'MCBIOS', kind: 'Poster',
          topic: 'Deep5hmC: Predicting genome-wide 5hmC landscape via multimodal deep learning model',
          award: 'MCBIOS 2024 Travel Fellowship' }
      ]
    },
    {
      place: 'Tampa, FL',
      lat: 27.9506, lng: -82.4572,
      talks: [
        { date: 'July 2023', venue: 'ICIBM', kind: 'Oral',
          topic: 'Integrated Spatial Multi-omics Analysis Based on MALDI Data' }
      ]
    }
  ];

  function esc(s) {
    return String(s).replace(/&/g, '&amp;').replace(/</g, '&lt;').replace(/>/g, '&gt;');
  }

  function card(p) {
    var h = '<div class="talk-tip__place">' + esc(p.place) + '</div>';
    for (var i = 0; i < p.talks.length; i++) {
      var t = p.talks[i];
      h += '<div class="talk-tip__item">';
      h += '<div class="talk-tip__meta">' + esc(t.date) + ' &middot; ' + esc(t.venue) + ' &middot; ' + esc(t.kind) + '</div>';
      h += '<div class="talk-tip__topic">' + esc(t.topic) + '</div>';
      if (t.award) h += '<div class="talk-tip__award">' + esc(t.award) + '</div>';
      h += '</div>';
    }
    return h;
  }

  var map = L.map('talkmap', { scrollWheelZoom: false, zoomControl: true });

  L.tileLayer('https://{s}.basemaps.cartocdn.com/light_all/{z}/{x}/{y}{r}.png', {
    attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors &copy; <a href="https://carto.com/attributions">CARTO</a>',
    subdomains: 'abcd',
    maxZoom: 18
  }).addTo(map);

  var pts = [];
  PLACES.forEach(function (p) {
    var n = p.talks.length;
    var m = L.circleMarker([p.lat, p.lng], {
      radius: 8 + (n - 1) * 3,
      color: '#ffffff',
      weight: 2,
      fillColor: '#52adc8',
      fillOpacity: 0.85
    }).addTo(map);

    var html = card(p);
    m.bindTooltip(html, { className: 'talk-tip', direction: 'top', offset: [0, -6], opacity: 1 });
    m.bindPopup(html, { className: 'talk-tip-popup', maxWidth: 300 });
    m.on('mouseover', function () { this.setStyle({ fillOpacity: 1, weight: 3 }); });
    m.on('mouseout', function () { this.setStyle({ fillOpacity: 0.85, weight: 2 }); });

    pts.push([p.lat, p.lng]);
  });

  map.fitBounds(L.latLngBounds(pts), { padding: [45, 45] });
  map.once('click', function () { map.scrollWheelZoom.enable(); });
})();
</script>
