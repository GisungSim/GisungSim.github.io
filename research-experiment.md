---
layout: home
permalink: /research-experiment/
published: true
---

<p style="font-size: 30px;"><b>Exploring the Quantum Frontier: The Generation of Squeezed States</b></p>

<p style="font-size: 24px;">The Generation of Squeezed States from Four-Wave Mixing</p>

With hard effort and trials, I have successfully generated a two-mode squeezed state of light via four-wave mixing!

It was the first accomplishment in Korea that two-mode squeezed light had been generated using atomic vapor, and overall, it was the second such achievement in the country across all methods

<figure style="width: 90%" class="align-center">
  <img src="/assets/images/squeezing-1.png" alt="">
  <figcaption>(left) Intensity difference squeezing at 100 kHz. (right) Intensity-difference noise versus total optical power at 100 kHz.</figcaption>
</figure>

I measured around 6 dB of intensity-difference squeezing, indicating that the noise power is suppressed by 75% beyond the standard quantum limit (a limit on measurement accuracy at quantum scales; or the maximum measurement accuracy achievable with classical states). In our experimental setup, the highest degree of squeezing occurred at 100 kHz, and the squeezing bandwidth's upper limit reached up to 2 MHz.

<figure style="width: 90%" class="align-center">
  <img src="/assets/images/squeezing-2.png" alt="">
  <figcaption>Geometry of the experiment and schematic of the double-lambda system.</figcaption>
</figure>

In this experiment, I utilized the double-lambda system of the D1 transition of <sup>85</sup>Rb. The strong coherence between the two ground states made from this scheme allows us to circumvent fundamental limitations to efficient squeezing, such as spontaneous emission [C. F. McCormick _et al_. PRA 78, 043816 (2008)].

<figure style="width: 90%" class="align-center">
  <img src="/assets/images/squeezing-3.png" alt="">
  <figcaption>(left) Probe transmission profile versus one-photon detuning. (right) Beam profile of the four-wave mixing beams with 6 dB of intensity difference squeezing.</figcaption>
</figure>

<p style="font-size: 24px;">Overcoming Challenges: From Start to the Achievement</p>

<b>Start from scratch: Over 99% of Electronic Noise Reduction</b> <br>
The initial challenge was the significant noise in my lab, which rendered my squeezing experiments virtually infeasible.

So my first task was suppressing the environmental (mainly electronic) noise. Firstly, I analyzed the circuit diagram of the detector to verify the noise source. And I realized the detector is particularly vulnerable to the RF electronic noise from the ground (I cannot attach the diagram because of the copyright) since it mainly consisted of many high-pass filters to the ground.

<figure style="width: 90%" class="align-center">
  <img src="/assets/images/squeezing-5.png" alt="">
  <figcaption>Noise spectra (left) before and (right) after my homemade noise filter!</figcaption>
</figure>

Then, I looked for solution of it. And I decided the best resolution is passive noise filters (yes, active noise filter might be better, but I have no time to learn and design it...) Since our interested squeezing bandwidth is from several kHz to MHz and I verified the strong noise source in lower MHz domain, I decided to make noise filter for around 1 MHz (and of course, another reason is that many papers look their squeezed state of light at 1 MHz).

Combining inductors, ferrite cores, and EMI filters properly, I made my homemade filter specialized to my experiment and successfully supressed the noise over 99%!

<b>Laser Power Amplification</b>

<b>Frequency Modulation</b>

<b>Beam Filtering</b>

<b>Four-Wave Mixing and Phase-Matching Condition</b>

<p style="font-size: 24px;">Looking Ahead</p>

