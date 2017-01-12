---
title       : LVZ Retreat, 2017 
subtitle    : 
author      : Mukarram Hossain
job         : University of Cambridge
framework   : revealjs        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : zenburn      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
revealjs:
theme: serif
transition: cube
center: "false"
knit        : slidify::knit2slides
---
  
## Subtype classification using lossless compression techniques 
<br></br>
**Mukarram Hossain**
<br></br>
Department of Veterinary Medicine  
University of Cambridge
<br></br>
LVZ Retreat, 2017 
<br></br>
<img src="assets/img/uc-colour.png" width="30%" style="border: 0px">&nbsp;


---
  
### Lossless compression 
  
<br><br></br></br>
`Lossless compression is a class of data compression algorithms that allows the original data to be perfectly reconstructed from the compressed data.`

--- 
  
### Subtype classification
  
- Viruses are often grouped into subtypes.
- Subtypes have wide implications on the following studies of viruses:
    - clinical
    - epidemiological
    - structural
    - functional
- Existing classification techniques mostly rely on alignments followed by phylogenetic and/or statistical algorithms.

---

### Alignment uncertainty - 1 

<img src="assets/img/ha.sp.png" width="65%" style="border: 0px">&nbsp;

---

### Alignment uncertainty - 2

<img src="assets/img/denv.sp.png" width="100%" style="border: 0px">&nbsp;

---

### Alignment-free classification

- Lossless compression techniques have shown promising results for biological sequence classification:
  - Begleiter et al. (2004)
  - Ferragina et al. (2007)

---
  
<br></br>
<img src="assets/img/comet_title.png" width="100%" style="border: 0px">&nbsp;

---
  
### COMET 
  
- COMET is an ultrafast alignment free subtyping tool
- Uses **P**rediction by **P**artial **M**atching (PPM)
- Initially designed for HIV-1
- COMET was tested on both synthetic (1090698) and clinical (10625) HIV datasets
- Sensitivity and specificity were comparable to or higher than:
    - REGA (de Oliveira *et al.*, 2005) and 
    - SCUEAL (Pond *et al.*, 2009)
- Detected and identified new recombinant forms

---

### PPM - model 

<img src="assets/img/ppm.png" width="80%" style="border: 0px">&nbsp;

---

### PPM - likelihoods

<img src="assets/img/ppm_prob.png" width="100%" style="border: 0px">&nbsp;

---

### COMET algorithm

- Builds variable-order Markov models for each reference sequence
- Given a query, COMET calculates log likelihood of observing a base at each positions
- This results in a matrix of likelihood values
- Subtype call is done using a decision tree

---

### The decision tree

<img src="assets/img/decision_tree.png" width="600px" height="650px" style="border: 0px">&nbsp;

---

### COMET - availability

- COMET is free to use via an [online](https://comet.lih.lu/) interface
- Stand-alone Java jar file can be requested from the author via <daniel.struck@lih.lu>

---

### pyCOMET

<img src="assets/img/pycomet.png" width="950px" height="650px" style="border: 0px">&nbsp;

---

### pyCOMET - results

<img src="assets/img/pycomet_results.png" width="100%" style="border: 0px">&nbsp;

---

### Classification using Neural networks

- *Neural networks* are computational system mimicking biological brain
- Consists of a cluster of neural unit organised in layers

<br></br>
<img src="assets/img/ann.jpg" width="40%" style="border: 0px">&nbsp;

---

### Classification using RNN

- Recurrent neural networks are networks with connections so that information can persist

<br></br>
<img src="assets/img/rnn.png" width="60%" style="border: 0px">&nbsp;

---

### Classification using lossless compression

- "*More accurate and more reliable*" and "*faster*" than current best methods.
- Robust, capable of identifying rare and novel recombinant forms.
- Results are consistent on short segments as well as whole genomes.
- Do not rely on alignments hence not biased by alignment uncertainty.
<br></br>
- Depends solely on the availability of complete reference sequence set

---

## Plans for 2017

---

<img src="assets/img/grad.png" width="60%" style="border: 0px">&nbsp;

---

<br></br>
<img src="assets/img/questions.jpg" width="600px" class="centred" style="margin: 10px 10px" />
  
