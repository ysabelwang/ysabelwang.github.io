---
layout: page
permalink: /aboutme/index.html
title: About me
---

##### About me
<p style="font-size: 14pt">
  Here you will find some of my background information. Click on each section below to expand or collapse.
</p>

***

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
    font-weight: 600;
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

  /* ---------- Education block styles ---------- */
  .edu-item {
    margin-bottom: 20px;
    padding: 12px 15px;
    border-radius: 6px;
    background-color: #fafafa;
    border-left: 4px solid #333;
    overflow: auto;
  }

  .edu-logo {
    float: left;
    margin-right: 15px;
  }

  .edu-logo img {
    width: 50px;
    height: auto;
  }

  .edu-body {
    overflow: hidden; /* clears float */
  }

  .edu-header {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    margin-bottom: 5px;
  }

  .edu-degree {
    font-weight: bold;
    font-size: 14px;
  }

  .edu-date {
    font-size: 12px;
    color: #666;
  }

  .edu-school {
    font-size: 13px;
    margin-bottom: 3px;
  }

  .edu-school-phd {
    font-size: 13px;
    margin-bottom: 3px;
    margin-left: 65px;
    text-indent: -65px;
  }

  /* Mobile layout for education items */
  @media (max-width: 600px) {
    .edu-item {
      display: flex;
      align-items: flex-start;
      gap: 12px;
      overflow: visible;
    }

    .edu-logo {
      float: none;
      margin-right: 0;
      flex-shrink: 0;
    }

    .edu-body {
      flex: 1;
      overflow: visible;
    }

    .edu-header {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      align-items: baseline;
      gap: 4px 8px;
      margin-bottom: 4px;
    }

    .edu-school,
    .edu-school-phd {
      margin-left: 0;
      text-indent: 0;
      line-height: 1.4;
    }
  }
</style>

<div class="collapsible-wrapper">

  <!-- BIO SECTION -->
  <div class="collapsible-section" id="background">
    <details open>
      <summary>BIO</summary>
      <div class="collapsible-content">
        <p style="font-size: 14pt">I am a third year PhD candidate studying Physical Oceanography in the MIT-WHOI Joint Program. I'm currently investigating the cross-scale variability of ocean processes in the Northwestern Atlantic where Gulf Stream meanders play a huge role in the oceanography. </p>

        <p style="font-size: 14pt">I was born and raised in Metro Manila, Philippines. Before moving to the US in 2021 to start graduate school, I worked for 3 years as a physical oceanography researcher after receiving a BS in Physics in 2018. In August of 2023 I graduated with a MS in Oceanography from Texas A&M University, where I was advised by  <a href="https://ocean.tamu.edu/people/profiles/faculty/dimarcosteve.html" target="_blank">Steve DiMarco</a>.</p>

        <p style="font-size: 14pt">Outside of school and research, I enjoy playing the guitar, powerlifting, reading, video games, and the occasional pro-wrestling show. I have a mini dachshund named Spamwise Hamgee.</p>
      </div>
    </details>
  </div>

  <!-- EDUCATION SECTION -->
  <div class="collapsible-section" id="education">
    <details>
      <summary>Education and Academic Background</summary>
      <div class="collapsible-content">

        <!-- PhD BLOCK -->
        <div class="edu-item">
          <div class="edu-logo">
            <img src="/images/mit-logo.svg" alt="MIT Logo">
          </div>

          <div class="edu-body">
            <div class="edu-header">
              <div class="edu-degree">PhD in Physical Oceanography</div>
              <div class="edu-date">2023</div>
            </div>

            <div class="edu-school-phd">
              Massachusetts Institute of Technology &amp; Woods Hole Oceanographic Institution
            </div>
          </div>
        </div>

        <!-- MS BLOCK -->
        <div class="edu-item">
          <div class="edu-logo">
            <img src="/images/tamu-logo.svg" alt="TAMU Logo">
          </div>

          <div class="edu-body">
            <div class="edu-header">
              <div class="edu-degree">MS Oceanography</div>
              <div class="edu-date">2021 – 2023</div>
            </div>

            <div class="edu-school">
              Texas A&amp;M University
            </div>
          </div>
        </div>

        <!-- BS BLOCK -->
        <div class="edu-item">
          <div class="edu-logo">
            <img src="/images/up-logo.svg" alt="UPD Logo">
          </div>

          <div class="edu-body">
            <div class="edu-header">
              <div class="edu-degree">BS in Physics</div>
              <div class="edu-date">2013 – 2018</div>
            </div>

            <div class="edu-school">
              University of the Philippines Diliman
            </div>
          </div>
        </div>

      </div>
    </details>
  </div>

  <!-- CV SECTION -->
  <div class="collapsible-section" id="cv">
    <details>
      <summary>CV (Last updated on: Dec. 4, 2025)</summary>
      <div class="collapsible-content">

        <div style="margin: 20px 0;">

          <!-- Scrollable PDF Viewer -->
          <div 
            style="
              width: 100%;
              height: 600px;
              overflow-y: scroll;
              border: 1px solid #ccc;
              border-radius: 6px;
            "
          >
            <embed 
              src="/files/ywang_cv.pdf#navpanes=0&zoom=page-width"
              type="application/pdf"
              width="100%"
              height="1200px"
              style="border: none;"
            />
          </div>

        </div>

      </div>
    </details>
  </div>

</div>
