---
layout: home
permalink: /research-experiment/
published: true
---

<p style="font-size: 30px;"><b>Beyond the Standard Quantum Limit: The Generation of Squeezed States</b></p>

<p style="font-size: 24px;"><b>The Generation of a Squeezed State from Four-Wave Mixing</b></p>

With hard effort and many trials, I have successfully generated a two-mode squeezed state of light via four-wave mixing with a diode laser!

This marks the first instance in Korea of generating two-mode squeezed light using atomic vapor, and the second accomplishment in Korea using any method!

<figure style="width: 90%" class="align-center">
  <img src="/assets/images/squeezing-1.png" alt="">
  <figcaption>Fig. 1. (left) Intensity difference squeezing at 100 kHz. (right) Intensity-difference noise versus total optical power at 100 kHz.</figcaption>
</figure>

I measured 6 dB of intensity-difference squeezing, indicating that the noise power is suppressed by 75% beyond the standard quantum limit (a limit on measurement accuracy at quantum scales; or the maximum measurement accuracy achievable with "classical" states). In our experimental setup, the highest degree of squeezing occurred at 100 kHz, and the squeezing bandwidth's upper limit reached up to 2 MHz.

<figure style="width: 90%" class="align-center">
  <img src="/assets/images/squeezing-2.png" alt="">
  <figcaption>Fig. 2. Geometry of the experiment and schematic of the double-lambda system.</figcaption>
</figure>

In this experiment, I utilized the double-lambda system of the D1 transition of <sup>85</sup>Rb (see Fig.2). The strong coherence between the two ground states made from this scheme allows us to circumvent fundamental limitations to efficient squeezing, such as spontaneous emission [C. F. McCormick _et al_. PRA 78, 043816 (2008)].

<figure style="width: 90%" class="align-center">
  <img src="/assets/images/squeezing-3.png" alt="">
  <figcaption>Fig. 3. (left) Probe transmission profile versus one-photon detuning. (right) Beam profile of the four-wave mixing beams with 6 dB of intensity difference squeezing.</figcaption>
</figure>

During the process of four-wave mixing, two photons of a single pump field are converted into a _pair of photons_, which are called probe and conjugate (Fig.2). Thus, probe-seed field obtain additional photons (but _cross-coupled_ and _jointly amplified_ with conjugate field), which we call _four-wave mixing gain_. Ideally, the degree of squeezing increases as the gain increases. However, there is a _tradeoff_ due to additional noise (mainly probe loss because probe is close to resonance) [M. T. Turnbull _et al_. PRA 88, 033845 (2013)]. Thus, in general, the optimum gain for squeezing ranges between 9-15 and this is true to my experiment (see Fig. 3).

In Fig. 3, you may notice the difference between the spatial mode profile of the probe and conjugate beams. I think it comes from the fact that probe is way more close to the resonance so that it experiences self-focusing and cross-phase modulation while the conjugate, which is far from the resonance, does not.

<p style="font-size: 24px;"><b>Overcoming Challenges: From Start to the Achievement</b></p>

<b>Start from scratch: Over 99% of Electronic Noise Reduction</b><br>
The initial challenge was the significant noise in my lab, which rendered my squeezing experiments virtually infeasible.

So my first task was suppressing the environmental (mainly electronic) noise. Initially, I analyzed the circuit diagram of the detector to verify the noise source. And I realized the detector is particularly vulnerable to the RF electronic noise from the ground (Unfortunately, due to copyright restrictions, I cannot attach the circuit diagram) since it mainly consisted of many high-pass filters to the ground.

<figure style="width: 90%" class="align-center">
  <img src="/assets/images/squeezing-5.png" alt="">
  <figcaption>Fig. 4. Noise spectra (left) before and (right) after my homemade noise filter!</figcaption>
</figure>

Then, I looked for a solution of it. And I decided the best resolution is passive noise filters (yes, active noise filter might be better, but I have no time to learn and design it...) Since our targeted squeezing bandwidth ranges from several kHz to MHz and I verified the strong noise source in lower MHz domain, I decided to make noise filter for around 1 MHz (and of course, another reason is that many papers look their squeezed state of light at 1 MHz).

Combining inductors, ferrite cores, and EMI filters properly, I made my homemade filter specialized to my experiment and successfully suppressed the noise by over 99%!

<b>Laser Power Amplification</b><br>
Since my diode laser emits only 40 mW, I need to amplify the laser power because four-wave mixing in the double-lambda system we utilized requires large detuning so that several mW is required (400 to 700 mW, typlically).

To achieve it, I made and operated a master oscillator power amplifier (MOPA) system with a tapered amplifier (with help of an other member, thanks Yejin!)

<figure style="width: 90%" class="align-center">
  <img src="/assets/images/squeezing-6.png" alt="">
  <figcaption>Fig. 5. (left) MOPA system in my setup. (right) Output power after MOPA system.</figcaption>
</figure>

After the power amplification, the power of the laser beam becomes 1.2 W (from 40 mW). The beam (which is named _pump_) is then sent through a single-mode optical fiber to clean up its spatial mode (with 60% of coupling efficiency!).

<b>Frequency Modulation</b><br>
But I still need another beam: probe seed, which is red-detuned from the pump (amplified laser source) as shown in Fig. 2. External field (that is, the probe-seed beam) should be injected to stimulate FWM beams to achieve strong quantum correlation between the FWM beams (which named _probe_ and _conjugate_, respectively).

Generally, acousto-optic modulator (AOM) is used for make probe-seed beam with good phase-locking between pump and probe-seed. Unfortunately, we don't have AOM having desired frequency shift spec. So I firstly tried to use another laser with phase-locking between pump laser (existed laser) and probe-seed laser (new laser). We succeeded to make lock-in signal but we wasn't able to do PID control since the laser controller did not allow the external modulation signal we made.

<figure style="width: 55%" class="align-center">
  <img src="/assets/images/squeezing-7.png" alt="">
  <figcaption>Fig. 6. EOM output signal taken by Fabry-Perrot interferometer.</figcaption>
</figure>

Thus we decided to use electro-optic modulator (EOM) and I build setup for EOM and operate it. And I succeeded to make probe-seed beam!

<b>Four-Wave Mixing and Phase-Matching Condition</b><br>
Now, every beam is ready. But we must satisfy _phase-matching condition_, which comes from both principles: conservation of energy and momentum, to successfully generate the desiring four-wave mixing signals. And energy condition has been satisfied as above. The rest is momentum, that is, _wave vector_.

<figure style="width: 55%" class="align-center">
  <img src="/assets/images/squeezing-8.png" alt="">
  <figcaption>Fig. 7. Phase-matching condition in my experiment.</figcaption>
</figure>

One might expect that the effective phase-matcing condition will be fulfilled at θ＝0 between the pump and probe-seed. However, the probe experiences an effective index of refraction larger than 1 as the probe is close to the resonance so that it experiences many dispersion occur near the resonance. In this situation, the effective phase-matching condition is fulfilled a finite angle θ (≠0) [M. T. Turnull _et al_. PRA 88, 033845 (2013)].

<figure style="width: 90%" class="align-center">
  <img src="/assets/images/squeezing-9.png" alt="">
  <figcaption>Fig. 8. Calculation of the phase-matching condition with a simple model for hot atomic vapor (thanks to Heewoo!).</figcaption>
</figure>

In my experiment, it is actually θ≈0.3 (and other papers have had the similar results).

The length of my cell is 12.5 mm, that is, the length of light-matter interaction is 12.5 mm. To make sure overapping the two beams (pump and probe-seed) along the entire length (otherwise it experiences strong loss), I chose the waist of pump and probe-seed as 550 μm and 330 μm, respectively.

<figure style="width: 55%" class="align-center">
  <img src="/assets/images/squeezing-10.png" alt="">
  <figcaption>Fig. 9. Beam profile of four-wave mixing; left, center, right beams are probe, pump, conjugate, respectively.</figcaption>
</figure>

Thereafter, I successfully generated desired four-wave mixing signals!

<b>Optimization of the Squeezing</b><br>
Of course, _Nothing Comes Easy_. I wasn't able to measure squeezing signal immediately. There had been many problems such as unexpected reflection and nonlinear phenomenon, pump scattering, significant fluctuation of four-wave mixing signals, cell scattering, to name a few. In particular, something not mentioned in papers...

But I dealt with it step by step, keeping in mind "I'm on the right track!" since I knows Nothing Comes Easy! And I know that I will eventually overcome it.

By careful modifying (namely, upgrading) my setup, changing the cell, suppress fluctuation of the signals by suppressing temperature fluctuation, resolving the cell scattering by implementing new heating system, optimizing phase-matching condition by fine controlling beam arrangement and shape, by fine tuning of laser frequency, I finally achieved it!

<figure style="width: 55%" class="align-center">
  <img src="/assets/images/squeezing-11.png" alt="">
  <figcaption>Fig. 10. The first squeezing I measured! I cannot forget the moment I measured it... Even my advisor also very excited of it.</figcaption>
</figure>

This was the first time of generation of squeezed state using atomic vapor in Korea!

Afterwards, I keep going to further optimization of squeezing. I optimized the squeezing by enhancing phase-matching conditions; improved detection efficiency by modifying the detecter with new photodetectors of higher quantum quantum efficiency (85% to 92%); minimized optical loss by filtering pump scattering by polarization, blocking other unwanted optical components, and fine-tuning the cell and setup alignment.

<figure style="width: 55%" class="align-center">
  <img src="/assets/images/squeezing-12.png" alt="">
  <figcaption>Fig. 11.</figcaption>
</figure>

<p style="font-size: 24px;">Looking Ahead</p>

