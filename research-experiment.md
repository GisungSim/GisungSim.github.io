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
  <figcaption>Fig. 1. (Left) Intensity difference squeezing at 100 kHz. Blue line, the standard quantum limit (SQL); red line, the four-wave mixing (FWM), that is, the squeezed state. (Right) Intensity-difference noise versus total optical power at 100 kHz.</figcaption>
</figure>

In this experiment, I achieved 6 dB of intensity-difference squeezing. This result indicates a suppression of noise power by 75% beyond the _standard quantum limit_ (a limit on measurement accuracy at quantum scales; or the maximum measurement accuracy achievable with "classical" states). In my setup, the maximum degree of squeezing was observed at 100 kHz, and the upper limit of the squeezing bandwidth extended to 2 MHz.

<figure style="width: 90%" class="align-center">
  <img src="/assets/images/squeezing-2.png" alt="">
  <figcaption>Fig. 2. Geometry of my experiment and schematic of the double-lambda system.</figcaption>
</figure>

I employed the double-lambda system in the D1 transition of <sup>85</sup>Rb for this experiment (see Fig. 2). The strong coherence between the two ground states created by this scheme enabled us to overcome fundamental limitations to efficient squeezing, such as spontaneous emission [C. F. McCormick _et al_. PRA 78, 043816 (2008)].

<figure style="width: 90%" class="align-center">
  <img src="/assets/images/squeezing-3.png" alt="">
  <figcaption>Fig. 3. (Left) Probe transmission profile versus one-photon detuning. (Right) Beam profile of the four-wave mixing beams with 6 dB of intensity difference squeezing.</figcaption>
</figure>

During the process of four-wave mixing, two photons of a single pump field are converted into a _pair of photons_, termed probe and conjugate (see Fig. 3). Consequently, the probe-seed field obtains additional photons (but _cross-coupled_ and _jointly amplified_ with the conjugate field), which we call _four-wave mixing gain_.

Ideally, the degree of squeezing increases with the gain. However, there is a _trade-off_ due to additional noise, primarily probe loss, as the probe experiences absorption since it is near the atomic resonance [M. T. Turnbull et al. PRA 88, 033845 (2013)]. Thus, in general, the optimum gain for squeezing ranges between 9-15 and this is true in my experiment (see Fig. 3).

In Fig. 3, you may notice the difference between the spatial modes of the probe and conjugate beams. I attribute this to the probe being closer to the resonance, leading to self-focusing and cross-phase modulation effects, unlike the conjugate beam, which is far from the resonance. And I verified this assumption by controlling atomic density and the pump power. The pump and probe are focused as the atomic density increses - self-focusing. The probe is moving as the pump power changed - cross-phase modulation.

<p style="font-size: 24px;"><b>Overcoming Challenges: From Start to the Achievement</b></p>

<b>Start from scratch: Over 99% of Electronic Noise Reduction</b><br>
The initial challenge in my lab was the significant electronic noise, which rendered my squeezing experiments virtually infeasible.

Therefore, my first task was suppressing the electronic noise. Initially, I analyzed the circuit diagram of the detector to identify the noise source. And I discovered the detector was particularly vulnerable to RF electronic noise from the ground. This vulnerability was mainly due to its design, which consisted of many high-pass filters connected to the ground (due to copyright restrictions, I cannot attach the circuit diagram here).

<figure style="width: 90%" class="align-center">
  <img src="/assets/images/squeezing-5.png" alt="">
  <figcaption>Fig. 4. Noise spectra (Left) before and (Right) after my homemade noise filter!</figcaption>
</figure>

Then, I looked for a solution for the noise issue. I concluded that the best resolution was to implement passive noise filters. Given that our targeted squeezing bandwidth ranges from several kHz to MHz, and after identifying a strong noise source in the lower MHz domain, I decided to create a noise filter centered around 1 MHz. 

To tailor a solution to my experiment's specific needs, I properly construct a customized homemade filter. This filter was remarkably successful, suppressing the noise over 99%!

<b>Laser Power Amplification</b><br>
Four-wave mixing in the double-lambda system requires large detuning and typically necessitates high power (over several hundred mW). However, the power of my diode laser was only 40 mW. So amplification system was making essential.

To address this, I constructed and operated a master oscillator power amplifier (MOPA) system with a tapered amplifier (with help of an other member, thanks Yejin!).

<figure style="width: 90%" class="align-center">
  <img src="/assets/images/squeezing-6.png" alt="">
  <figcaption>Fig. 5. (Left) MOPA system in my setup. (Right) Output power after MOPA system.</figcaption>
</figure>

After the power amplification, the laser beam's power was increased to 1.2 W (from 40 mW). This beam, named _pump_, was then sent through a single-mode optical fiber to clean up its spatial mode (with 60% of coupling efficiency!).

<b>Frequency Modulation</b><br>
I also needed another beam: the probe-seed, which is red-detuned from the pump (the amplified laser source), as shown in Fig. 2. To stimulate FWM beams and achieve strong quantum correlation between the beams (named _probe_ and _conjugate_, respectively), an external field, namely the probe-seed beam, should be injected.

Typically, an acousto-optic modulator (AOM) is used to create a probe-seed beam in good phase-locking between the pump and probe-seed. Unfortunately, we didn't have an AOM with the necessary frequency shift specifications. So I tried to use another laser and tried to implement phase-locking with the existing pump laser. But we were unable to make error signal since our laser controller was incompatible with the external modulation signal we had created.

<figure style="width: 55%" class="align-center">
  <img src="/assets/images/squeezing-7.png" alt="">
  <figcaption>Fig. 6. EOM output signal taken by Fabry-Perrot interferometer.</figcaption>
</figure>

Thus, we decided to use an electro-optic modulator (EOM). I constructed a setup for the EOM and successfully operated it, which enabled me to create the required probe-seed beam.

<b>Four-Wave Mixing and Phase-Matching Condition</b><br>
Now, every beam is ready. However, to generate the desired four-wave mixing signals, we must satisfy the _phase-matching condition_, which arises from the principles of conservation of energy and momentum. The energy condition has already been met, as described above. The remaining consideration is momentum, that is, the _wave vector_.

<figure style="width: 55%" class="align-center">
  <img src="/assets/images/squeezing-8.png" alt="">
  <figcaption>Fig. 7. Phase-matching condition in my experiment.</figcaption>
</figure>

One might expect that effective phase-matching condition would be satisfied at θ＝0 of the cross angle between the pump and probe-seed. However, since the probe is close to the resonance (see Fig. 7) and experiences dispersion in this region, it encounters an effective index of refraction larger than 1. Consequently, the effective phase-matching condition is fulfilled at a finite angle θ (>0), as evidenced in the study by M. T. Turnbull _et al_. [PRA 88, 033845 (2013)].

<figure style="width: 90%" class="align-center">
  <img src="/assets/images/squeezing-9.png" alt="">
  <figcaption>Fig. 8. Calculation for intensity distribution of the phase-matching condition with a simple model for hot Rubidium vapor (thanks to Heewoo!).</figcaption>
</figure>

In my experiment, this angle was approximately θ ≈ 0.3, a result consistent with similar findings in other papers.

The length of our rubidium cell is 12.5 mm. To ensure overlapping of the two beams (pump and probe-seed) along the entire length (otherwise the probe will experience strong loss), I selected the waist sizes of the pump and probe-seed beams to be 550 μm and 330 μm, respectively.

<figure style="width: 55%" class="align-center">
  <img src="/assets/images/squeezing-10.png" alt="">
  <figcaption>Fig. 9. Beam profile of four-wave mixing; left, center, right beams are probe, pump, conjugate, respectively.</figcaption>
</figure>

Consequently, I successfully generated the desired four-wave mixing beams!

<b>Optimization of the Squeezing</b><br>
Of course, _Nothing Comes Easy_. Initially, I couldn't immediately measure the squeezing after generating the twin FWM beams. I faced many challenges, such as unexpected nonlinear phenomena, significant fluctuations in the four-wave mixing signals, cell window scattering, pump scattering, optical losses, and low quantum efficiency of the detector, among others – issues often not mentioned in papers.

But I dealt with these problems step by step. Such as implementing modifications and enhancements to my experimental setup, stabilizing temperature to suppress the signal fluctuations, resolving the cell window scattering with an advanced heating system, reducing the pump scattering through polarization and spatial filtering, and minimizing the optical losses by using more suitable optical components and arrangements.

Moreover, another crucial aspect was optimizing the phase-matching condition to successfully generate the squeezed state. By fine-tuning the frequency of each pump and probe-seed beam, adjusting their spatial arrangement and modes, and controlling other parameters like atomic density, I eventually achieved squeezing!!

<figure style="width: 55%" class="align-center">
  <img src="/assets/images/squeezing-11.png" alt="">
  <figcaption>Fig. 10. The first squeezing I measured! (Blue line, the standard quantum limit (SQL); red line, the four-wave mixing (FWM), that is, the squeezed state) I cannot forget the moment I measured it... Even my advisor also very excited of it.</figcaption>
</figure>

As such, whenever I encounter a problem, I tackle it methodically, constantly reminding myself, "I'm on the right track!" I firmly believe that persistence and determination will overcome any obstacle, as long as I continue to persevere and never give up.


Afterwards, I keep going to further optimize the squeezing. I achieved it by further optimizing the phase-matching conditions; improving detection efficiency by modifying the detector with new photodetectors that have higher quantum efficiency (increased from 85% to 92%); minimizing optical loss by further filtering out pump scattering, blocking other unwanted signals, and fine-tuning the alignment of the setup.

<figure style="width: 55%" class="align-center">
  <img src="/assets/images/squeezing-12.png" alt="">
  <figcaption>Fig. 11. Futher optimized squeezing signal (Blue line, the standard quantum limit (SQL); red line, the squeezed state (FWM)).</figcaption>
</figure>

<p style="font-size: 24px;">Looking Ahead</p>

My remarkable achievement is now leading to various exciting projects:
- Quantum-enhanced electric field sensing with a Rydberg atom
- Quantum-enhanced optical magnetometry
- Quantum information processing with continuous variables: Covariant quantum measurement of a two-mode squeezed state with dual homodyne detection
