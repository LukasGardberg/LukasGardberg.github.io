---
title: "Thesis Audio Examples"
layout: post
mathjax: true
---

This post contains audio samples generated using various versions of DiffWave and PriorGrad. The left column contains samples from LJSpeech, and the right sampels from LibriTTS. For details see the thesis: (TODO: add link)

---

### Reference samples

Ground Truth
{% include embed-audio.html src="/assets/audio_examples/LJ/ground-truth-LJ050-0277.wav" %} {% include embed-audio.html src="/assets/audio_examples/Libri/ground-truth-3922_715_000069_000001.wav" %}

Griffin Lim
{% include embed-audio.html src="/assets/audio_examples/LJ/GL-LJ050-0277.wav" %} {% include embed-audio.html src="/assets/audio_examples/Libri/GL-3922_715_000069_000001.wav" %}

---

#### Schedules

Linear $$\beta_T=0.05$$
{% include embed-audio.html src="/assets/audio_examples/LJ/diffwave-LJ050-0277.wav" %} {% include embed-audio.html src="/assets/audio_examples/Libri/diffwave-3922_715_000069_000001.wav" %}

Scaled Linear $$\beta_T=0.05$$
{% include embed-audio.html src="/assets/audio_examples/LJ/diffwave-scaled-0.05-LJ050-0277.wav" %} {% include embed-audio.html src="/assets/audio_examples/Libri/diffwave-scaled-0.05-3922_715_000069_000001.wav" %}

Scaled Linear $$\beta_T=0.02$$
{% include embed-audio.html src="/assets/audio_examples/LJ/diffwave-scaled-0.02-LJ050-0277.wav" %} {% include embed-audio.html src="/assets/audio_examples/Libri/diffwave-scaled-0.02-3922_715_000069_000001.wav" %}

Cosine
{% include embed-audio.html src="/assets/audio_examples/LJ/diffwave-cos-LJ050-0277.wav" %} {% include embed-audio.html src="/assets/
audio_examples/Libri/diffwave-cos-3922_715_000069_000001.wav" %}

Inverse Quadratic
{% include embed-audio.html src="/assets/audio_examples/LJ/diffwave-custom-LJ050-0277.wav" %} {% include embed-audio.html src="/assets/audio_examples/Libri/diffwave-custom-3922_715_000069_000001.wav" %}

---

#### Importance Sampling (IS)
<!--- Note: "Uniform" is the same model as "Linear $$\beta_T=0.05$$".

Uniform 
{% include embed-audio.html src="/assets/audio_examples/LJ/diffwave-LJ050-0277.wav" %} {% include embed-audio.html src="/assets/audio_examples/Libri/diffwave-3922_715_000069_000001.wav" %} --->

Note: "Uniform" is the same model as "Linear $$\beta_T=0.05$$".

Uniform (fast)
{% include embed-audio.html src="/assets/audio_examples/LJ/diffwave-fast-LJ050-0277.wav" %} {% include embed-audio.html src="/assets/audio_examples/Libri/diffwave-fast-3922_715_000069_000001.wav" %}

IS
{% include embed-audio.html src="/assets/audio_examples/LJ/diffwave-IS-LJ050-0277.wav" %} {% include embed-audio.html src="/assets/audio_examples/Libri/diffwave-IS-3922_715_000069_000001.wav" %}

IS (fast)
{% include embed-audio.html src="/assets/audio_examples/LJ/diffwave-IS-fast-LJ050-0277.wav" %} {% include embed-audio.html src="/assets/audio_examples/Libri/diffwave-IS-fast-3922_715_000069_000001.wav" %}

---

#### Noise Prior

Note: Samples are of higher volume as a consequence of the inference process. Use a volume of around 50% for a fair comparison.

PriorGrad
{% include embed-audio.html src="/assets/audio_examples/LJ/priorgrad-LJ050-0277.wav" %} {% include embed-audio.html src="/assets/audio_examples/Libri/priorgrad-3922_715_000069_000001.wav" %}

PriorGrad (fast)
{% include embed-audio.html src="/assets/audio_examples/LJ/priorgrad-fast6-LJ050-0277.wav" %} {% include embed-audio.html src="/assets/audio_examples/Libri/priorgrad-fast-3922_715_000069_000001.wav" %}

---

#### Model Size

Base + IQ + IS
{% include embed-audio.html src="/assets/audio_examples/LJ/diffwave-custom-IS-LJ050-0277.wav" %} {% include embed-audio.html src="/assets/audio_examples/Libri/diffwave-custom-IS-3922_715_000069_000001.wav" %}

Base + IQ + IS (fast)
{% include embed-audio.html src="/assets/audio_examples/LJ/diffwave-custom-IS-fast-LJ050-0277.wav" %} {% include embed-audio.html src="/assets/audio_examples/Libri/diffwave-custom-IS-fast-3922_715_000069_000001.wav" %}

$$\\$$

Small
{% include embed-audio.html src="/assets/audio_examples/LJ/diffwave-small-LJ050-0277.wav" %} {% include embed-audio.html src="/assets/audio_examples/Libri/diffwave-small-3922_715_000069_000001.wav" %}

Small + IQ + IS
{% include embed-audio.html src="/assets/audio_examples/LJ/diffwave-custom-IS-small-LJ050-0277.wav" %} {% include embed-audio.html src="/assets/audio_examples/Libri/diffwave-custom-IS-small-3922_715_000069_000001.wav" %}

Small (fast)
{% include embed-audio.html src="/assets/audio_examples/LJ/diffwave-small-fast-LJ050-0277.wav" %} {% include embed-audio.html src="/assets/audio_examples/Libri/diffwave-small-fast-3922_715_000069_000001.wav" %}

Small + IQ + IS (fast)
{% include embed-audio.html src="/assets/audio_examples/LJ/diffwave-custom-IS-small-fast-LJ050-0277.wav" %} {% include embed-audio.html src="/assets/audio_examples/Libri/diffwave-custom-IS-small-fast-3922_715_000069_000001.wav" %}

---

#### Longer Training

HiFi-GAN
{% include embed-audio.html src="/assets/audio_examples/LJ/hifigan-LJ050-0277.wav" %} {% include embed-audio.html src="/assets/audio_examples/Libri/hifigan-3922_715_000069_000001.wav" %}

DiffWave 2.5M
{% include embed-audio.html src="/assets/audio_examples/LJ/diffwave2.5m-LJ050-0277.wav" %} {% include embed-audio.html src="/assets/audio_examples/Libri/diffwave2.5m-3922_715_000069_000001.wav" %}

DiffWave 2.5M (fast)
{% include embed-audio.html src="/assets/audio_examples/LJ/diffwave2.5m-fast-LJ050-0277.wav" %} {% include embed-audio.html src="/assets/audio_examples/Libri/diffwave2.5m-fast-3922_715_000069_000001.wav" %}

DiffWave 2.5M + IQ + IS
{% include embed-audio.html src="/assets/audio_examples/LJ/diffwave2.5m-custom-IS-LJ050-0277.wav" %} {% include embed-audio.html src="/assets/audio_examples/Libri/diffwave2.5m-custom-IS-3922_715_000069_000001.wav" %}

DiffWave 2.5M + IQ + IS (fast)
{% include embed-audio.html src="/assets/audio_examples/LJ/diffwave2.5m-custom-IS-fast-LJ050-0277.wav" %} {% include embed-audio.html src="/assets/audio_examples/Libri/diffwave2.5m-custom-IS-fast-3922_715_000069_000001.wav" %}
