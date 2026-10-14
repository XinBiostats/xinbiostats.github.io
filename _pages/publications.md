---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<style>
.pub-h {
  font-size: 1.1em;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: #6b7177;
  border-bottom: 1px solid #e6e8ea;
  padding-bottom: 0.4em;
  margin: 2em 0 1em;
}
/* ---- Selected publications: sliding cards ---- */
.fpub-carousel { position: relative; }

.fpub-arrow {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  z-index: 3;
  width: 2.4em;
  height: 2.4em;
  padding: 0 0 0.12em;
  display: flex;
  align-items: center;
  justify-content: center;
  border: 1px solid #dfe2e4;
  border-radius: 50%;
  background: #fff;
  color: #5b6166;
  font-size: 1.2em;
  line-height: 1;
  cursor: pointer;
  box-shadow: 0 2px 10px rgba(30, 40, 50, 0.17);
  transition: background 0.15s ease, color 0.15s ease, border-color 0.15s ease, opacity 0.15s ease;
}
.fpub-arrow--prev { left: -14px; }
.fpub-arrow--next { right: -14px; }
@media (max-width: 64em) {
  .fpub-arrow--prev { left: 6px; }
  .fpub-arrow--next { right: 6px; }
}
.fpub-arrow:hover:not(:disabled) { background: #52adc8; border-color: #52adc8; color: #fff; }
.fpub-arrow:disabled { opacity: 0; pointer-events: none; }

.fpub-track {
  display: flex;
  gap: 1.4em;
  overflow-x: auto;
  scroll-snap-type: x mandatory;
  scroll-behavior: smooth;
  -webkit-overflow-scrolling: touch;
  scrollbar-width: none;
  padding-bottom: 0.3em;
  margin-bottom: 2.2em;
}
.fpub-track::-webkit-scrollbar { display: none; }

.fpub {
  flex: 0 0 calc((100% - 2 * 1.4em) / 3);
  scroll-snap-align: start;
  display: flex;
  flex-direction: column;
  border: 1px solid #e6e8ea;
  border-radius: 6px;
  overflow: hidden;
  background: #fff;
  text-decoration: none !important;
  color: inherit !important;
  transition: transform 0.18s ease, box-shadow 0.18s ease, border-color 0.18s ease;
}
@media (max-width: 64em) { .fpub { flex-basis: calc((100% - 1.4em) / 2); } }
@media (max-width: 37.5em) { .fpub { flex-basis: 100%; } }

.fpub:hover, .fpub:focus {
  transform: translateY(-3px);
  box-shadow: 0 8px 22px rgba(30, 40, 50, 0.13);
  border-color: #d2d6d9;
  text-decoration: none !important;
  color: inherit !important;
}
.fpub img {
  display: block;
  width: 100%;
  aspect-ratio: 4 / 3;
  object-fit: contain;
  background: #fff;
  border-bottom: 1px solid #edeff1;
  margin: 0;
}
.fpub__body {
  padding: 0.9em 1em 1.1em;
  display: flex;
  flex-direction: column;
  flex: 1 1 auto;
}
.fpub__venue {
  font-size: 0.72em;
  font-weight: 600;
  letter-spacing: 0.07em;
  text-transform: uppercase;
  color: #52adc8;
  margin-bottom: 0.45em;
}
.fpub__title {
  font-size: 0.95em;
  line-height: 1.35;
  font-weight: 700;
  margin: 0 0 0.5em;
  color: #3b4045;
}
.fpub__authors {
  font-size: 0.78em;
  color: #6b7177;
  margin: 0 0 0.6em;
  line-height: 1.4;
}
.fpub__blurb {
  font-size: 0.82em;
  line-height: 1.5;
  color: #5b6166;
  margin: 0 0 1em;
}
.fpub__cta {
  margin-top: auto;
  font-size: 0.78em;
  font-weight: 600;
  color: #52adc8;
}
.fpub:hover .fpub__cta { color: #3d8299; }

/* ---- Full list ---- */
.pub-list { padding-left: 1.4em; }
.pub-list li { margin-bottom: 0.85em; line-height: 1.5; }
</style>

<h2 class="pub-h">Selected Publications</h2>

<div class="fpub-carousel">

<button type="button" class="fpub-arrow fpub-arrow--prev" id="fpubPrev" aria-label="Previous publications">&#8249;</button>
<button type="button" class="fpub-arrow fpub-arrow--next" id="fpubNext" aria-label="Next publications">&#8250;</button>

<div class="fpub-track" id="fpubTrack">

  <a class="fpub" href="https://doi.org/10.1101/gr.281260.125" target="_blank" rel="noopener">
    <img src="{{ '/images/publications/featured-genome-research-2026.png' | relative_url }}" alt="Figure 1 from the GraphScrDom paper" loading="lazy">
    <div class="fpub__body">
      <div class="fpub__venue">Genome Research &middot; 2026</div>
      <h3 class="fpub__title">Reference-informed spatial domain detection using weak supervision for spatial transcriptomics</h3>
      <p class="fpub__authors"><strong>Ma, X.</strong>, Jin, W., Lu, Q., et al.</p>
      <p class="fpub__blurb">A weakly supervised framework that borrows annotated reference tissue to detect spatial domains in new spatial transcriptomics samples.</p>
      <span class="fpub__cta">View paper &rarr;</span>
    </div>
  </a>

  <a class="fpub" href="https://doi.org/10.1038/s41467-025-59487-7" target="_blank" rel="noopener">
    <img src="{{ '/images/publications/featured-nature-communications-2025.png' | relative_url }}" alt="Figure 2 from the Sami framework paper" loading="lazy">
    <div class="fpub__body">
      <div class="fpub__venue">Nature Communications &middot; 2025</div>
      <h3 class="fpub__title">Spatial mapping of the brain metabolome, lipidome and glycome</h3>
      <p class="fpub__authors">Clarke, H.A.<sup>&dagger;</sup>, <strong>Ma, X.</strong><sup>&dagger;</sup>, Shedlock, C.J.<sup>&dagger;</sup>, et al.</p>
      <p class="fpub__blurb">Metabolites, lipids and glycans resolved from a single tissue section and assembled into one spatial multi-omics atlas of the brain.</p>
      <span class="fpub__cta">View paper &rarr;</span>
    </div>
  </a>

  <a class="fpub" href="https://doi.org/10.1038/s42255-025-01242-9" target="_blank" rel="noopener">
    <img src="{{ '/images/publications/featured-nature-metabolism-2025.png' | relative_url }}" alt="Figure 1 from the MetaVision3D paper" loading="lazy">
    <div class="fpub__body">
      <div class="fpub__venue">Nature Metabolism &middot; 2025</div>
      <h3 class="fpub__title">AI-driven framework to map the brain metabolome in three dimensions</h3>
      <p class="fpub__authors"><strong>Ma, X.</strong><sup>&dagger;</sup>, Shedlock, C.J.<sup>&dagger;</sup>, Medina, T.<sup>&dagger;</sup>, et al.</p>
      <p class="fpub__blurb">A deep learning pipeline that reconstructs the brain metabolome in three dimensions from serial mass spectrometry imaging sections.</p>
      <span class="fpub__cta">View paper &rarr;</span>
    </div>
  </a>

  <a class="fpub" href="https://doi.org/10.1093/bioinformatics/btae528" target="_blank" rel="noopener">
    <img src="{{ '/images/publications/featured-bioinformatics-2024.png' | relative_url }}" alt="Figure 1 from the Deep5hmC paper" loading="lazy">
    <div class="fpub__body">
      <div class="fpub__venue">Bioinformatics &middot; 2024</div>
      <h3 class="fpub__title">Deep5hmC: predicting genome-wide 5-hydroxymethylcytosine landscape via a multimodal deep learning model</h3>
      <p class="fpub__authors"><strong>Ma, X.</strong>, Thela, S.R., Zhao, F., et al.</p>
      <p class="fpub__blurb">A multimodal deep learning model that predicts genome-wide 5hmC modification by combining DNA sequence with matched epigenetic data.</p>
      <span class="fpub__cta">View paper &rarr;</span>
    </div>
  </a>

</div>

</div>

<script>
(function () {
  var track = document.getElementById('fpubTrack');
  var prev = document.getElementById('fpubPrev');
  var next = document.getElementById('fpubNext');
  if (!track || !prev || !next) return;

  function step() {
    var card = track.querySelector('.fpub');
    if (!card) return track.clientWidth;
    var gap = parseFloat(getComputedStyle(track).columnGap || '0') || 0;
    return card.getBoundingClientRect().width + gap;
  }

  function sync() {
    var max = track.scrollWidth - track.clientWidth;
    var atStart = track.scrollLeft <= 1;
    var atEnd = track.scrollLeft >= max - 1;
    prev.disabled = atStart;
    next.disabled = atEnd;
    var hide = max <= 1;
    prev.style.display = hide ? 'none' : '';
    next.style.display = hide ? 'none' : '';
  }

  prev.addEventListener('click', function () { track.scrollBy({ left: -step(), behavior: 'smooth' }); });
  next.addEventListener('click', function () { track.scrollBy({ left: step(), behavior: 'smooth' }); });
  track.addEventListener('scroll', sync, { passive: true });
  window.addEventListener('resize', sync);
  window.addEventListener('load', sync);
  sync();
})();
</script>

<h2 class="pub-h">Peer-Reviewed Publications</h2>

<p><sup>&dagger;</sup> indicates co-first author.</p>

<ol class="pub-list">

<li>
<strong>Ma, X.</strong>, Allison, D., Macedo, J.K.A., et al.
<em>Machine learning-based prediction of clinical outcomes in glioblastoma using glycomics features</em>.
<em>Computational and Structural Biotechnology Journal</em> (2026).
</li>

<li>
<strong>Ma, X.</strong>, Jin, W., Lu, Q., et al.
<em>Reference-Informed Detection of Spatial Domains Using Weak Supervision for Spatial Transcriptomics</em>.
<em>Genome Research</em> (2026).
</li>

<li>
Hawkinson, T.R., Liu, Z., Ribas, R.A., et al., <strong>Ma, X.</strong>, et al.
<em>Hyperglycosylation is a metabolic driver of Alzheimer's disease</em>.
<em>Nature Metabolism</em> (2026).
</li>

<li>
Ribas, R., Tang, Q., Caffee, S., et al., <strong>Ma, X.</strong>, Chen, L., Sun, R., et al.
<em>Mass Spectrometry-based Spatial Imaging of the Cochlea</em>.
<em>Journal of the American Society for Mass Spectrometry</em> (2026).
</li>

<li>
Clarke, H.A.<sup>&dagger;</sup>, <strong>Ma, X.</strong><sup>&dagger;</sup>, Shedlock, C.J.<sup>&dagger;</sup>, et al.
<em>Spatial mapping of the brain metabolome lipidome and glycome</em>.
<em>Nature Communications</em>, 16, 4373 (2025).
</li>

<li>
<strong>Ma, X.</strong><sup>&dagger;</sup>, Shedlock, C.J.<sup>&dagger;</sup>, Medina, T.<sup>&dagger;</sup>, et al.
<em>AI-driven framework to map the brain metabolome in three dimensions</em>.
<em>Nature Metabolism</em> (2025).
</li>

<li>
Clarke, H.A., Hawkinson, T.R., Clarke, H., et al., <strong>Ma, X.</strong>, et al.
<em>Glycogen drives tumour initiation and progression in lung adenocarcinoma</em>.
<em>Nature Metabolism</em> (2025).
</li>

<li>
<strong>Ma, X.</strong>, Thela, S.R., Zhao, F., et al.
<em>Deep5hmC: predicting genome-wide 5-hydroxymethylcytosine landscape via a multimodal deep learning model</em>.
<em>Bioinformatics</em>, 40(9), btae528 (2024).
</li>

<li>
Zhao, F., <strong>Ma, X.</strong>, Yao, B., et al.
<em>Scada: A novel statistical method for differential analysis of single-cell chromatin accessibility sequencing data</em>.
<em>PLOS Computational Biology</em>, 20(8) (2024).
</li>

</ol>

<h2 class="pub-h">Manuscripts Under Revision</h2>

<ol class="pub-list">

<li>
Rodriguez-Palma, E., Gomez, K., Calderon-Rivera, A., et al., <strong>Ma, X.</strong>, et al.
<em>A peptidomimetic inhibitor of moesin alleviates chronic pain by suppressing NaV1.7 and NaV1.8 channels</em>.
<em>Science Translational Medicine</em> (under revision).
</li>

<li>
Guarnieri, J.W., Maghsoudi, Z., Kim, J., et al., <strong>Ma, X.</strong>, et al.
<em>Guardians of the Mitochondria: Space Mitochondria 2.0 Systemic Analysis Reveals Bioenergetic Dysregulation Across Species</em>.
<em>Cell</em> (under revision).
</li>

</ol>

<h2 class="pub-h">Manuscripts Under Review</h2>

<ol class="pub-list">

<li>
Jin, W., Zhao, F., <strong>Ma, X.</strong>, et al.
<em>DeepCNet: An interpretable deep learning model for inferring cell type-specific promoter-enhancer interactions from single-cell multiome data</em>.
<em>Nature Communications</em> (under review).
</li>

<li>
Liu, Z.<sup>&dagger;</sup>, <strong>Ma, X.</strong><sup>&dagger;</sup>, Ribas, R., et al.
<em>Metabolic Coherence of the Mouse Brain</em>.
<em>Cell</em> (under review).
</li>

<li>
Medina, T., Qui&ntilde;ones, S., Liu, Z., et al., <strong>Ma, X.</strong>, et al.
<em>A multi-organ spatial metabolomic atlas of exercising mice reveals neuronal Complex I as a convergent and sufficient axis for tau pathology reduction in PS19</em>.
<em>Science</em> (under review).
</li>

</ol>
