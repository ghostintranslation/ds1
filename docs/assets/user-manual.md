---
pdf_options:
  format: A4
  margin:
    top: 0
    right: 0
    bottom: 0
    left: 0
  printBackground: true
  displayHeaderFooter: false
---

<style>
/* CSS for premium A4 User Manual PDF */

/* Global styles */
body, .markdown-body {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
  color: #1e293b !important;
  background-color: #ffffff !important;
  line-height: 1.6;
  font-size: 11pt;
}

h1, h2, h3, h4 {
  color: #0f172a !important;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
  font-weight: 600;
  margin-top: 1.2em;
  margin-bottom: 0.4em;
}

h1 {
  font-size: 22pt;
  border-bottom: 2px solid #cbd5e1;
  padding-bottom: 0.3em;
  margin-top: 0;
  text-transform: uppercase;
}

h2 {
  font-size: 16pt;
  border-bottom: 1px solid #e2e8f0;
  padding-bottom: 0.2em;
}

h3 {
  font-size: 12pt;
}

p, li {
  color: #334155;
  font-size: 11pt;
}

ul, ol {
  margin-top: 0.4em;
  margin-bottom: 0.8em;
  padding-left: 1.5em;
}

li {
  margin-bottom: 0.3em;
}

a {
  color: #0284c7 !important;
  text-decoration: none;
}

a:hover {
  text-decoration: underline;
}

/* Code and syntax highlighting */
code {
  background-color: #f1f5f9 !important;
  color: #0f172a !important;
  padding: 0.2em 0.4em;
  border-radius: 4px;
  font-family: ui-monospace, SFMono-Regular, SF Mono, Menlo, Consolas, monospace;
  font-size: 9pt;
}

pre {
  background-color: #f8fafc !important;
  border: 1px solid #e2e8f0;
  padding: 12px;
  border-radius: 6px;
  overflow: auto;
  margin: 1em 0;
}

pre code {
  background-color: transparent !important;
  padding: 0;
  font-size: 9pt;
}

/* Table styles */
table {
  border-collapse: collapse;
  width: 100%;
  margin: 1.2em 0;
  font-size: 9.5pt;
}

th, td {
  padding: 8px 10px;
  border: 1px solid #cbd5e1 !important;
  text-align: left;
}

th {
  background-color: #f1f5f9 !important;
  color: #0f172a !important;
  font-weight: 600;
}

tr:nth-child(even) {
  background-color: #f8fafc !important;
}

/* Page structural styles */
.cover-page {
  width: 100vw;
  height: 100vh;
  box-sizing: border-box;
  background-image: linear-gradient(rgba(0, 0, 0, 0.35), rgba(0, 0, 0, 0.35)), url('./ds1.jpg');
  background-size: cover;
  background-position: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 0 20mm;
  color: #ffffff !important;
  text-align: center;
  break-after: page;
  page-break-after: always;
}

.cover-brand {
  font-size: 16pt;
  font-weight: 300;
  color: #ffffff !important;
  letter-spacing: 4px;
  text-transform: uppercase;
  margin-bottom: 20px;
  margin-top: 0;
}

.cover-title-group h1.cover-title {
  font-size: 92pt !important;
  color: #ffffff !important;
  font-weight: 800;
  letter-spacing: 2px;
  border-bottom: none;
  margin: 0;
  padding: 0;
}

.cover-subtitle {
  font-size: 20pt;
  font-weight: 300;
  margin-top: 15px;
  color: #e2e8f0;
}

.toc-page, .page-body {
  width: 100vw;
  height: 100vh;
  box-sizing: border-box;
  margin: 0;
  padding: 20mm 30mm 30mm 30mm; /* Extra bottom space for footer */
  position: relative;
  break-after: page;
  page-break-after: always;
  background-color: #ffffff;
}

/* Table of Contents page specific styles */
.toc-heading {
  font-size: 22pt;
  margin-top: 0;
  margin-bottom: 1.5em;
  border-bottom: 2px solid #0f172a;
  padding-bottom: 0.4em;
  text-transform: uppercase;
}

.toc-list {
  list-style: none;
  padding: 0;
  margin: 0;
}

.toc-list li {
  display: flex;
  align-items: baseline;
  margin-bottom: 16px;
  font-size: 12pt;
}

.toc-title {
  font-weight: 500;
  color: #334155;
}

.toc-dots {
  flex-grow: 1;
  border-bottom: 1px dotted #94a3b8;
  margin: 0 12px;
  position: relative;
  top: -4px;
}

.toc-page-num {
  font-weight: 600;
  color: #0f172a;
}

/* Custom footer style */
.page-footer {
  position: absolute;
  bottom: 15mm;
  left: 20mm;
  right: 20mm;
  display: flex;
  justify-content: space-between;
  font-size: 8pt;
  color: #64748b;
  font-family: -apple-system, BlinkMacSystemFont, sans-serif;
  border-top: 1px solid #e2e8f0;
  padding-top: 8px;
}

/* Printing styling to enforce A4 sizing and zero margins */
@media print {
  @page {
    size: A4;
    margin: 0; /* Let HTML containers specify boundaries */
  }

  body, .markdown-body {
    background-color: #ffffff !important;
    padding: 0 !important;
    margin: 0 !important;
  }

  .cover-page, .toc-page, .page-body {
    width: 210mm;
    height: 297mm;
    margin: 0;
    box-sizing: border-box;
  }
}
</style>

<div class="cover-page">
  <div class="cover-title-group">
    <p class="cover-brand">Ghost In Translation</p>
    <h1 class="cover-title">DS1</h1>
    <p class="cover-subtitle">1.0.X</p>
  </div>
</div>

<div class="toc-page">
  <!-- Table of Contents Section -->
  <h2 class="toc-heading">Table of Contents</h2>
  <ul class="toc-list">
    <li>
      <span class="toc-title">1. Introduction</span>
      <span class="toc-dots"></span>
      <span class="toc-page-num">3</span>
    </li>
    <li>
      <span class="toc-title">2. Installation</span>
      <span class="toc-dots"></span>
      <span class="toc-page-num">4</span>
    </li>
    <li>
      <span class="toc-title">3. Controls and CV Inputs</span>
      <span class="toc-dots"></span>
      <span class="toc-page-num">5</span>
    </li>
    <li>
      <span class="toc-title">4. Menu & Navigation</span>
      <span class="toc-dots"></span>
      <span class="toc-page-num">6</span>
    </li>
    <li>
      <span class="toc-title">5. The 16 Algorithms</span>
      <span class="toc-dots"></span>
      <span class="toc-page-num">7</span>
    </li>
    <li>
      <span class="toc-title">6. MIDI Implementation</span>
      <span class="toc-dots"></span>
      <span class="toc-page-num">9</span>
    </li>
    <li>
      <span class="toc-title">7. Firmware Update</span>
      <span class="toc-dots"></span>
      <span class="toc-page-num">10</span>
    </li>
    <li>
      <span class="toc-title">8. Troubleshooting</span>
      <span class="toc-dots"></span>
      <span class="toc-page-num">11</span>
    </li>
  </ul>
  <!-- Page footer with page number 2 -->
  <div class="page-footer">
    <span>DS1 User Manual</span>
    <span>Page 2</span>
  </div>
</div>

<div class="page-body">
  <!-- Section 1: Introduction -->
  <h1>1. Introduction</h1>

  <p>DS1 is a multi-algorithm Drum Synthesizer module based on my Motherboard platform.</p>

  <h2>Features</h2>

  <ul>
    <li>16 algorithms</li>
    <li>32 bit float DSP</li>
    <li>48kHz 32 bit audio</li>
    <li>MIDI TRS Type A IN and OUT</li>
    <li>Auto calibration</li>
    <li>Either-way power</li>
  </ul>
  
  <h2>Technical Specifications</h1>

  <ul>
    <li><strong>Module Width</strong>: 8 HP</li>
    <li><strong>Depth</strong>: 45 mm</li>
    <li><strong>Power Consumption</strong>:
      <ul>
        <li><strong>+12V</strong>: 75 mA</li>
        <li><strong>-12V</strong>: 3.5 mA</li>
      </ul>
    </li>
    <li><strong>CV Input Range</strong>: 0V to 5V</li>
  </ul>
  
  <!-- Page footer with page number 3 -->
  <div class="page-footer">
    <span>DS1 User Manual</span>
    <span>Page 3</span>
  </div>
</div>

<div class="page-body">
  <!-- Section 2: Installation -->
  <h1>2. Installation</h1>

  <p>Turn off and disconnect your Eurorack case from AC mains power before installing this module. Connect the supplied power ribbon cable to the module and your busboard. This module is equiped with either-way power, so no magic smoke will be released if you plug it in backwards.</p>
  
  <!-- Page footer with page number 4 -->
  <div class="page-footer">
    <span>DS1 User Manual</span>
    <span>Page 4</span>
  </div>
</div>

<div class="page-body">
  <!-- Section 3: Controls and CV Inputs -->
  <h1>3. Controls and CV Inputs</h1>

  <p>All CV inputs read voltages between 0 and 5V.</p>

  <h2>Knobs</h2>
  <ul>
    <li><strong>Pitch</strong>: Sets the base pitch/tuning for the voice.</li>
    <li><strong>Decay</strong>: Controls the envelope decay time.</li>
    <li><strong>Tone</strong>: Controls the brightness of the sound.</li>
    <li><strong>Drive</strong>: Controls the gain of the drive/waveshaper stage.</li>
    <li><strong>Param 1</strong>: Controls the primary sound synthesis parameter.</li>
    <li><strong>Param 2</strong>: Controls the secondary sound synthesis parameter.</li>
  </ul>

  <h2>CV Inputs</h2>
  <ul>
    <li><strong>CV Pitch</strong>: Controls the pitch of the voice.</li>
    <li><strong>CV Decay</strong>: Controls the decay of the voice envelope.</li>
    <li><strong>CV Accent</strong>: Controls the accent level of the voice.</li>
    <li><strong>CV Trigger</strong>: Triggers the voice.</li>
    <li><strong>CV Param 1</strong>: Controls the primary sound synthesis parameter.</li>
    <li><strong>CV Param 2</strong>: Controls the secondary sound synthesis parameter.</li>
    <li><strong>CV Select</strong>: Selects the voice.</li>
  </ul>

  <h2>Navigation Button</h2>
  <ul>
    <li><strong>SEL button</strong>:
      <ul>
        <li><strong>Short Press</strong>: Manual trigger.</li>
        <li><strong>Long Press (1 second)</strong>: Enters algorithm selection mode. </li>
      </ul>
    </li>
  </ul>
  
  <!-- Page footer with page number 5 -->
  <div class="page-footer">
    <span>DS1 User Manual</span>
    <span>Page 5</span>
  </div>
</div>

<div class="page-body">
  <!-- Section 4: Menu & Navigation -->
  <h1>4. Menu & Navigation</h1>

  <h2>Normal Play Mode</h2>
  <p>In normal play mode:</p>
  <ul>
    <li>The <strong>8 LEDs at the top</strong> display real-time levels of the control inputs and the main audio output.</li>
  </ul>

  <h2>Algorithm Selection Mode</h2>
  <p>To change the active sound algorithm:</p>
  <ol>
    <li><strong>Enter Menu</strong>: Long press the <strong>SEL button</strong>. All 8 top LEDs will turn solid <strong>Blue</strong>, except for the active selection.</li>
    <li><strong>Read Active Selection</strong>: The active selection is shown by two blinking <strong>Green</strong> LEDs:
      <ul>
        <li><strong>Bank Indicator</strong> (one of the first 4 LEDs)</li>
        <li><strong>Algorithm Indicator</strong> (one of the last 4 LEDs)</li>
      </ul>
    </li>
    <li><strong>Change Algorithm</strong>: Tap the <strong>SEL button</strong> to cycle to the next algorithm.</li>
    <li><strong>Save & Exit</strong>: After <strong>5 seconds</strong> of inactivity, the module saves your choice and returns to play mode automatically.</li>
  </ol>
  
  <!-- Page footer with page number 6 -->
  <div class="page-footer">
    <span>DS1 User Manual</span>
    <span>Page 6</span>
  </div>
</div>

<div class="page-body">
  <!-- Section 5: The 16 Algorithms (Bank 1 & 2) -->
  <h1>5. The 16 Algorithms</h1>

  <p>The module contains 16 algorithms. Below is an overview of what each algorithm does and what the <strong>Param 1</strong> and <strong>Param 2</strong> knobs control.</p>

  <h2>Bank 1</h2>
  <table>
    <thead>
      <tr>
        <th style="width: 6%">#</th>
        <th style="width: 38%">Sound Description</th>
        <th style="width: 28%">Param 1 Control</th>
        <th style="width: 28%">Param 2 Control</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>1</td>
        <td><strong>Kick 1</strong>: Dual-operator warm FM kick with rumble style sub.</td>
        <td>Rumble amount</td>
        <td>Pitch Sweep Drop Depth</td>
      </tr>
      <tr>
        <td>2</td>
        <td><strong>Kick 2</strong>: Deep sine kick with FM attack punch and pitch sweep.</td>
        <td>FM Transient Punch Amount</td>
        <td>Pitch Sweep Drop Depth</td>
      </tr>
      <tr>
        <td>3</td>
        <td><strong>Kick 3</strong>: Aggressive square-wave kick.</td>
        <td>Pitch Sweep Duration</td>
        <td>Pitch Sweep Drop Depth</td>
      </tr>
      <tr>
        <td>4</td>
        <td><strong>Kick 4</strong>: 909 style dual sine/triangle oscillator kick.</td>
        <td>Pitch Sweep Duration</td>
        <td>Pitch Drop Depth</td>
      </tr>
    </tbody>
  </table>

  <h2>Bank 2</h2>
  <table>
    <thead>
      <tr>
        <th style="width: 6%">#</th>
        <th style="width: 38%">Sound Description</th>
        <th style="width: 28%">Param 1 Control</th>
        <th style="width: 28%">Param 2 Control</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>1</td>
        <td><strong>Hi-Hat</strong>: 808 style and 909 sample combination.</td>
        <td>Metallic Frequency Ratio & Spread</td>
        <td>Fader from synthesized to sample</td>
      </tr>
      <tr>
        <td>2</td>
        <td>TBD</td>
        <td>TBD</td>
        <td>TBD</td>
      </tr>
      <tr>
        <td>3</td>
        <td><strong>Shaker</strong>: Physical shaker simulation.</td>
        <td>Jitter speed</td>
        <td>Grit and resonance</td>
      </tr>
      <tr>
        <td>4</td>
        <td><strong>Cymbal</strong>: 808 style and 909 sample combination.</td>
        <td>Metallic Pitch Sweep Range</td>
        <td>Fader from synthesized to sample</td>
      </tr>
    </tbody>
  </table>
  
  <!-- Page footer with page number 7 -->
  <div class="page-footer">
    <span>DS1 User Manual</span>
    <span>Page 7</span>
  </div>
</div>

<div class="page-body">
  <!-- Section 5: The 16 Algorithms (Continued: Bank 3 & 4) -->
  <h2>Bank 3</h2>
  <table>
    <thead>
      <tr>
        <th style="width: 6%">#</th>
        <th style="width: 38%">Sound Description</th>
        <th style="width: 28%">Param 1 Control</th>
        <th style="width: 28%">Param 2 Control</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>1</td>
        <td><strong>Clap</strong>: Classic pulsed noise.</td>
        <td>Pulses spacing</td>
        <td>Tail decay</td>
      </tr>
      <tr>
        <td>2</td>
        <td><strong>Tokyo Bell</strong>: Life is simple. You make choices and you don't look back.</td>
        <td>Mallet Strike Pitch & Transient</td>
        <td>Resonance Feedback Decay & Harmonics</td>
      </tr>
      <tr>
        <td>3</td>
        <td><strong>Rings</strong>: Physical modeling similar to the famous Rings by MI.</td>
        <td>Resonator Modal Structure & Spacing</td>
        <td>Strike Position</td>
      </tr>
      <tr>
        <td>4</td>
        <td><strong>Tom</strong>: FM synthesis with dynamic triangle modulator and wavefolder saturation.</td>
        <td>FM Index & Sweep</td>
        <td>Body Resonance & Tail Ambience</td>
      </tr>
    </tbody>
  </table>

  <h2>Bank 4</h2>
  <table>
    <thead>
      <tr>
        <th style="width: 6%">#</th>
        <th style="width: 38%">Sound Description</th>
        <th style="width: 28%">Param 1 Control</th>
        <th style="width: 28%">Param 2 Control</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>1</td>
        <td><strong>Gong</strong>: 4-operator FM inharmonic metallic.</td>
        <td>FM Modulation Index</td>
        <td>Inharmonic Wash Index</td>
      </tr>
      <tr>
        <td>2</td>
        <td><strong>FM Synth</strong>: Phase modulation voice.</td>
        <td>Modulator Frequency Multiplier</td>
        <td>Phase Modulation Index Depth</td>
      </tr>
      <tr>
        <td>3</td>
        <td><strong>Acid Bass</strong>: 303 style bass.</td>
        <td>Filter Envelope Sweep Depth</td>
        <td>Filter Resonance</td>
      </tr>
      <tr>
        <td>4</td>
        <td><strong>Dual Osc</strong>: Disconant synth voice.</td>
        <td>Waveform</td>
        <td>Detune Amount</td>
      </tr>
    </tbody>
  </table>
  
  <!-- Page footer with page number 8 -->
  <div class="page-footer">
    <span>DS1 User Manual</span>
    <span>Page 8</span>
  </div>
</div>


<div class="page-body">
  <!-- Section 7: MIDI Implementation -->
  <h1>7. MIDI Implementation</h1>

  <p>DS1 listens to and transmits on <strong>Channel 1</strong>.</p>

  <h2>Control Change (CC) Mapping</h2>
  <ul>
    <li><strong>CC 1</strong>: Pitch</li>
    <li><strong>CC 2</strong>: Decay</li>
    <li><strong>CC 3</strong>: Tone</li>
    <li><strong>CC 4</strong>: Drive</li>
    <li><strong>CC 5</strong>: Param 1</li>
    <li><strong>CC 6</strong>: Param 2</li>
    <li><strong>CC 7</strong>: Algorithm select</li>
  </ul>

  <!-- Page footer with page number 10 -->
  <div class="page-footer">
    <span>DS1 User Manual</span>
    <span>Page 9</span>
  </div>
</div>

<div class="page-body">
  <!-- Section 8: Firmware Update -->
  <h1>8. Firmware Update</h1>

  <p>The firmware update process is as follows:</p>

  <ol>
    <li><strong>Power Off the Module</strong>: Disconnect the module from power.</li>
    <li><strong>Press and hold BOOTSEL</strong>: Locate the physical <strong>BOOTSEL</strong> button on the microcontroller (Pico 2) on the back of the module, and hold it down.</li>
    <li><strong>Connect to Computer</strong>: While holding the <strong>BOOTSEL</strong> button, connect the Pico 2 to your computer via a USB cable.</li>
    <li><strong>Release BOOTSEL</strong>: Once the USB cable is plugged in, release the button. The Pico 2 will mount on your computer as a USB mass storage drive.</li>
    <li><strong>Transfer the Firmware</strong>: Locate the compiled firmware file <code>firmware/ds1.ino.uf2</code>. Drag and drop (or copy) the <code>.uf2</code> file onto the drive.</li>
    <li><strong>Automatic Reboot</strong>: The Pico 2 will write the new firmware to its flash memory, automatically eject/unmount, and reboot with the updated firmware running.</li>
  </ol>

  <!-- Page footer with page number 11 -->
  <div class="page-footer">
    <span>DS1 User Manual</span>
    <span>Page 10</span>
  </div>
</div>

<div class="page-body">
  <!-- Section 9: Troubleshooting -->
  <h1>9. Troubleshooting</h1>

  <h2>No Sound Output</h2>
  <ul>
    <li>Verify that the eurorack power ribbon cable is connected correctly.</li>
    <li>Make sure your audio cable is patched securely.</li>
    <li>Switch off and switch on the module.</li>
  </ul>
  
  <!-- Page footer with page number 12 -->
  <div class="page-footer">
    <span>DS1 User Manual</span>
    <span>Page 11</span>
  </div>
</div>