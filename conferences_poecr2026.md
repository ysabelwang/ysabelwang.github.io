---
layout: page
permalink: /conferences/poecr2026.html
title: 2026 Physical Oceanography Early Career Research Symposium
---
##### 2026 Physical Oceanography Early Career Research Symposium
<style>
  /* ---------- Collapsible blocks ---------- */
  .collapsible-wrapper {
    font-family: Quicksand, sans-serif;
    margin: 0;
    padding: 0;
  }

  .collapsible-section {
    max-width: 800px;
    margin: 20px auto;
  }

  .collapsible-section details {
    border: 1px solid #ddd;
    border-radius: 6px;
    background-color: #fafafa;
    margin-bottom: 16px;
    overflow: hidden;
  }

  .collapsible-section summary {
    padding: 10px 14px;
    font-size: 20px;
    font-weight: 300;
    cursor: pointer;
    list-style: none;
  }

  .collapsible-section summary::-webkit-details-marker {
    display: none;
  }

  .collapsible-section details[open] summary {
    border-bottom: 1px solid #ddd;
  }

  .collapsible-content {
    padding: 12px 16px 16px 16px;
    font-size: 14pt;
  }

  /* Optional: small indicator on the right */
  .collapsible-section summary::after {
    content: "▾";
    float: right;
    font-size: 0.9em;
  }

  .collapsible-section details[open] summary::after {
    content: "▴";
  }

  /* PDF insert */
  .pdf-link {
    display: block;
    text-decoration: none;
  }

  .pdf-preview embed {
    width: 100%;
    height: 100%;
    display: block;
    pointer-events: none;
  }

  .figure-link {
  text-decoration: none;
  color: inherit;
  display: block;

  .indented {
  text-indent: 2em;   /* or 30px */
}
}

  /* Let wide equations scroll horizontally instead of getting clipped on narrow/mobile screens */
  .katex-display {
    display: block;
    overflow-x: auto;
    overflow-y: hidden;
    -webkit-overflow-scrolling: touch;
    padding-bottom: 6px;
  }

  .katex-display > .katex {
    white-space: nowrap;
  }

  /* References */
  .ref-list {
    font-size: 14pt;
    padding-left: 0;
    list-style: none;
  }

  .ref-list li {
    margin-bottom: 12px;
    padding-left: 2em;
    text-indent: -2em;
  }
</style>
<div class="collapsible-wrapper">

  <!-- Summary -->
  <div class="collapsible-section" id="summary">
    <details open>
      <summary>Summary</summary>
      <div class="collapsible-content">
        <p style="font-size: 14pt">This work has two aims: (1) to accurately correct Surface Water and Ocean Topography (SWOT) altimetry measurements for internal tides using in situ observations from the mission's calibration/validation (cal/val) period in 2023, and (2) to use the corrected SWOT product to investigate submesoscale processes. 
        
        My progress to date addresses Objective 1. I am characterizing the behavior of internal tides at Cape Hatteras - a region where the various current systems like the Gulf Stream, fronts, eddies, and steep topography interact - using bottom-pressure and roundtrip acoustic travel time measurements from an array of current and pressure sensor equipped inverted echo sounders (<a href="https://doi.org/10.3389/fmars.2019.00232" target="_blank">CPIES</a>).</p>
      </div>
    </details>
  </div>

  <!-- SWOT and internal tides -->
  <div class="collapsible-section" id="swot_internal_tides">
    <details>
      <summary>How do internal tides affect SWOT measurements?</summary>
      <div class="collapsible-content">
        <p style="font-size: 14pt">SWOT is a wide-swath altimetry mission designed to resolve sea surface height (SSH) at submesoscale spatial resolutions - something conventional nadir altimeters have not been able to do. At these scales, however, SWOT's SSH signal is not purely a signature of geostrophic processes: it also contains expressions of internal tides (ITs). ITs have horizontal wavelengths (tens to hundreds of km) and surface SSH signatures (centimeters) that overlap with those of submesoscale ocean processes, so their signal must be identified and removed before the SWOT product can be used to study submesoscale dynamics.</p>

        <p style="font-size: 14pt" class="indented">The standard approach for removing IT signals from SWOT is to subtract a prediction of the coherent IT - i.e., the part of the IT that is phase-locked to, and therefore predictable from, the astronomical tide. The predictions are made by <a href="https://ingria.ceoas.oregonstate.edu/fossil/HRET/doc/tip/README.md" target="_blank">HRET (High Resolution Empirical Tides model)</a>, which uses decades of SSH records to estimate the coherent IT globally (Zaron, 2019). HRET performs well in many regions, but it cannot predict the incoherent portion of the IT which, as described below, is substantial in dynamically active regions such as Cape Hatteras. Quantifying that incoherent residual with independent in situ observations, and understanding where and why HRET's correction falls short, is the motivation for this work.</p>
      </div>
    </details>
  </div>

  <!-- Cape Hatteras complexity -->
  <div class="collapsible-section" id="cape_hatteras_complexity">
    <details>
      <summary>Why are internal tides at Cape Hatteras complex?</summary>
      <div class="collapsible-content">
        <p style="font-size: 14pt">Internal tides (ITs) form in stratified water when the barotropic tide - in which the entire water column moves nearly uniformly - encounters bottom topography. ITs propagate along density surfaces with amplitudes of tens of meters, in contrast to their centimeters of surface displacement.</p>

        <p style="font-size: 14pt" class="indented">Coherent ITs are predictable: their phase does not change with time relative to the astronomical tide, so an IT that is coherent at location <em>x</em> and time <em>t</em> can be used to predict the IT at that same location at any other time. This predictability is how HRET works. Incoherent ITs are not phase-locked to the barotropic tide and cannot be represented by a fixed set of tidal sinusoids. Knowing the incoherent IT at one time provides little information about its state beyond the local decorrelation timescale. In the North Atlantic, this timescale is only 5 days (Lahaye et al., 2024).</p>

        <p style="font-size: 14pt" class="indented">Incoherence arises when the water an IT propagates through varies faster than the tidal period, scattering the IT's phase and amplitude unpredictably. This occurs a lot at Cape Hatteras, as it's where the Gulf Stream separates from the continental shelf, so the region is constantly evolving with strong, meandering fronts and currents, all superimposed on steep shelf-break topography. This combination of energetic background flow and variable topography at Cape Hatteras results in ITs frequently becoming incoherent. The sea level variance associated with this incoherence, which in the North Atlantic is <em>55%</em>, is not predicted by HRET.</p>
      </div>
    </details>
  </div>

  <!-- CPIES -->
  <div class="collapsible-section" id="cpies">
    <details>
      <summary>CPIES to the rescue</summary>
      <div class="collapsible-content">
        <p style="font-size: 14pt">A conventional subsurface mooring is not a practical way to observe the Cape Hatteras environment, as the Gulf Stream can knock over or damage a moored instrument string. Current and pressure sensor equipped inverted echo sounders (CPIES) sidestep this problem: they sit on the seafloor (mostly) away from the energetic flow above. CPIES arrays have been used to characterize ITs and circulation in other energetic current systems, including the Kuroshio (Donohue et al., 2010) and the Antarctic Circumpolar Current in Drake Passage (Donohue et al., 2016).</p>

        <p style="font-size: 14pt" class="indented">Each CPIES combines two measurements to recover the IT signal through the full water column. Bottom pressure ($$p_{bottom}$$) records the weight of the water column directly above the sensor, which is essentially a measurement of the barotropic tide. The roundtrip acoustic travel time ($$\tau$$) is the time for a sound pulse to travel from the instrument to the surface and back; because sound speed depends on temperature and salinity, $$\tau$$ is sensitive to the mode-1 baroclinic structure of the water column. Converting $$p_{bottom}$$ to an equivalent travel time lets us estimate and remove the portion of $$\tau$$ due to the barotropic tide, leaving a residual, $$\tau_{res}$$, that reflects the IT.</p>

        <p style="font-size: 14pt" class="indented">Separating $$\tau_{res}$$ into its coherent ($$\tau_{res,\,coh}$$) and incoherent ($$\tau_{res,\,icoh}$$) parts then only requires harmonic fitting: because $$\tau_{res,\,coh}$$ is predictable, it can be fit with sinusoids using the classical harmonic analysis package <a href="https://www.eoas.ubc.ca/~rich/" target="_blank">T_TIDE</a> (Pawlowicz et al., 2002). Subtracting that from $$\tau_{res}$$ gives $$\tau_{res,\,icoh}$$.</p>
      </div>
    </details>
  </div>

  <!-- Vertical structure impact -->
  <div class="collapsible-section" id="vertical_structure">
    <details>
      <summary>Estimating the IT impact on vertical structure</summary>
      <div class="collapsible-content">
        <p style="font-size: 14pt">This section of converting $$\tau_{res}$$ into a physical displacement of the water column follows the transfer-function approach of Li et al. (2009).</p>

        <p style="font-size: 14pt" class="indented">Each CPIES samples $$\tau$$ hourly. Applying a 2-day low-pass filter removes all IT variability and anything else varying on two days or less, leaving $$\tau_{lp}$$. Each value of $$\tau_{lp}$$ corresponds to a background water column density profile, $$\rho_{bg}(z)$$, at least as an estimate of its general shape. This $$\tau_{lp}$$ and $$\rho_{bg}$$ relationship is the gravest empirical mode, or GEM, look-up table (Meinen &amp; Watts, 2000).</p>

        <p style="font-size: 14pt" class="indented">If most of the perturbation an IT makes to $$\rho_{bg}$$ projects onto the first baroclinic (mode-1) vertical structure - i.e., the water column moves up or down together, with the largest displacement centered at the pycnocline - then the shape of that displacement can be found by solving the mode-1 eigenvalue problem for a flat bottom and rigid lid (e.g., Gill, 1982):</p>

        <p style="font-size: 14pt">
        $$
        \frac{d^2 W_n}{dz^2} + \frac{N^2(z)}{c_n^2}\,W_n = 0, \qquad W_n(0) = W_n(H) = 0
        $$
        </p>

        <p style="font-size: 14pt" class="indented">where $$N(z)$$ is the stratification represented by buoyancy frequency profile, $$H$$ is the water depth, and $$W_1$$ and $$c_1$$ are the vertical structure function and eigenspeed of mode 1. Once $$W_1$$ is known, $$\rho_{bg}$$ is displaced by a range of arbitrary amplitudes along that shape, $$\tau$$ is recalculated through each displaced profile, and the resulting anomaly $$\tau_{anom}$$ is plotted against displacement amplitude. This relationship is luckily linear, so its slope defines a transfer function $$T$$ that converts a change in $$\tau$$ (in seconds) directly into a change in vertical displacement (in meters).</p>

        <p style="font-size: 14pt" class="indented">Applying $$T$$ to $$\rho_{bg}$$ with amplitudes set by the internal tide at a given time ($$\tau_{res}$$, $$\tau_{res,\,coh}$$, and/or $$\tau_{res,\,icoh}$$) then yields an estimate of the mode-1 displacement of the water column due to the internal tide. Integrating that displacement sterically gives the corresponding sea surface height anomaly - the quantity compared directly against HRET.</p>
      </div>
    </details>
  </div>

  <!-- Ongoing work -->
  <div class="collapsible-section" id="ongoing_work">
    <details>
      <summary>Ongoing work</summary>
      <div class="collapsible-content">
        <p style="font-size: 14pt"><strong>1. Can I assume a flat bottom?</strong></p>
        <p style="font-size: 14pt" class="indented">The eigenvalue problem above assumes a flat bottom and rigid lid, which greatly simplifies both the math and the processing. I am currently diagnosing whether that assumption is appropriate at each CPIES site. Following the topographic criticality framework of Cacchione et al. (2002), the diagnostic at each site is $$\epsilon(t)$$, the ratio of the local topographic slope to the IT's own characteristic slope in the background water column at time $$t$$:</p>

        <p style="font-size: 14pt">
        $$
        \epsilon(t) = \frac{|\nabla h|}{s(t)}, \qquad s(t) = \sqrt{\dfrac{\omega^2 - f^2}{N^2(z,t) - \omega^2}}
        $$
        </p>

        <p style="font-size: 14pt" class="indented">where $$|\nabla h|$$ is the bottom slope, $$\omega$$ is the tidal frequency, $$f$$ is the Coriolis frequency, and $$N(z,t)$$ is the local buoyancy frequency. A site is subcritical for $$\epsilon < 1$$, critical for $$\epsilon \approx 1$$, and supercritical for $$\epsilon > 1$$; the flat-bottom assumption is best justified where topography stays subcritical.</p>

        <p style="font-size: 14pt"><strong>2. Producing a lookup table of background profiles</strong></p>
        <p style="font-size: 14pt" class="indented">My next step is to build a GEM look-up table linking each $$\tau_{lp}$$ to a $$\rho_{bg}$$ that can then be perturbed by the IT components of $$\tau_{res}$$. This builds on the hydrographic and CPIES work compiled for the Processes Driving Exchange at Cape Hatteras (PEACH) program (Andres, 2020); the corresponding Part 2 report is not yet publicly archived &mdash; contact <a href="mailto:mandres@whoi.edu">mandres@whoi.edu</a> for a copy.</p>
      </div>
    </details>
  </div>

  <!-- References -->
  <div class="collapsible-section" id="references">
    <details>
      <summary>References</summary>
      <div class="collapsible-content">
        <ul class="ref-list">
          <li>Andres, M. (2020). <em>Processes Driving Exchange at Cape Hatteras (PEACH) PIESs and AP Technical Report &ndash; Part 1</em> (Version 1) [Data set]. Zenodo. <a href="https://doi.org/10.5281/zenodo.4793402" target="_blank">https://doi.org/10.5281/zenodo.4793402</a></li>
          <li>Cacchione, D. A., Pratson, L. F., &amp; Ogston, A. S. (2002). The shaping of continental slopes by internal tides. <em>Science, 296</em>(5568), 724&ndash;727. <a href="https://doi.org/10.1126/science.1069803" target="_blank">https://doi.org/10.1126/science.1069803</a></li>
          <li>Donohue, K. A., Watts, D. R., Tracey, K. L., Greene, A. D., &amp; Kennelly, M. (2010). Mapping circulation in the Kuroshio Extension with an array of current and pressure recording inverted echo sounders. <em>Journal of Atmospheric and Oceanic Technology, 27</em>(3), 507&ndash;527. <a href="https://doi.org/10.1175/2009JTECHO686.1" target="_blank">https://doi.org/10.1175/2009JTECHO686.1</a></li>
          <li>Donohue, K. A., Tracey, K. L., Watts, D. R., Chidichimo, M. P., &amp; Chereskin, T. K. (2016). Mean Antarctic Circumpolar Current transport measured in Drake Passage. <em>Geophysical Research Letters, 43</em>(22), 11760&ndash;11767. <a href="https://doi.org/10.1002/2016GL070319" target="_blank">https://doi.org/10.1002/2016GL070319</a></li>
          <li>Gill, A. E. (1982). <em>Atmosphere&ndash;Ocean Dynamics</em>. Academic Press.</li>
          <li>Li, Q., Farmer, D. M., Duda, T. F., &amp; Ramp, S. (2009). Acoustical measurement of nonlinear internal waves using the inverted echo sounder. <em>Journal of Atmospheric and Oceanic Technology, 26</em>(10), 2228&ndash;2242. <a href="https://doi.org/10.1175/2009JTECHO652.1" target="_blank">https://doi.org/10.1175/2009JTECHO652.1</a></li>
          <li>Meinen, C. S., &amp; Watts, D. R. (2000). Vertical structure and transport on a transect across the North Atlantic Current near 42&deg;N: Time series and mean. <em>Journal of Geophysical Research, 105</em>(C9), 21869&ndash;21892. <a href="https://doi.org/10.1029/2000JC900097" target="_blank">https://doi.org/10.1029/2000JC900097</a></li>
          <li>Morrow, R., Fu, L.-L., Ardhuin, F., Benkiran, M., Chapron, B., Cosme, E., d'Ovidio, F., Farrar, J. T., Gille, S. T., Lapeyre, G., Le Traon, P.-Y., Pascual, A., Ponte, A., Qiu, B., Rascle, N., Ubelmann, C., Wang, J., &amp; Zaron, E. D. (2019). Global observations of fine-scale ocean surface topography with the Surface Water and Ocean Topography (SWOT) mission. <em>Frontiers in Marine Science, 6</em>, Article 232. <a href="https://doi.org/10.3389/fmars.2019.00232" target="_blank">https://doi.org/10.3389/fmars.2019.00232</a></li>
          <li>Pawlowicz, R., Beardsley, B., &amp; Lentz, S. (2002). Classical tidal harmonic analysis including error estimates in MATLAB using T_TIDE. <em>Computers &amp; Geosciences, 28</em>(8), 929&ndash;937. <a href="https://doi.org/10.1016/S0098-3004(02)00013-4" target="_blank">https://doi.org/10.1016/S0098-3004(02)00013-4</a></li>
          <li>Zaron, E. D. (2019). Baroclinic tidal sea level from exact-repeat mission altimetry. <em>Journal of Physical Oceanography, 49</em>(1), 193&ndash;210. <a href="https://doi.org/10.1175/JPO-D-18-0127.1" target="_blank">https://doi.org/10.1175/JPO-D-18-0127.1</a></li>
        </ul>
      </div>
    </details>
  </div>

</div>