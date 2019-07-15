---
layout: page
title: 
permalink: /
pubs:
    - title:    "Model reduction of a parametrized scalar hyperbolic conservation law using displacement interpolation" 
      author:   "D. Rim and K.T Mandli"
      arxiv:    "https://arxiv.org/abs/1805.05938"
      journal:  "Preprint"
      github:   "http://github.com/dsrim/mr_burgers1d"
      year:     "2018"

    - title:    "Dimensional splitting of hyperbolic partial differential
                 equations using the Radon transform" 
      author:   "D. Rim"
      journal:  "SIAM J. Sci. Comput."
      numbers:  "**40** (6), A4184–A4207"
      arxiv:   "https://arxiv.org/abs/1705.03609"
      url:      "https://epubs.siam.org/doi/abs/10.1137/17M1135633"
      doi:      "https://doi.org/10.1137/17M1135633"
      year:     "2018"

    - title:    "Displacement interpolation using monotone rearrangement" 
      author:   "D. Rim and K.T Mandli"
      journal:  "SIAM/ASA J. Uncertainty Quantification"
      numbers:  "**6** (4), 1503-1531"
      arxiv:    "https://arxiv.org/abs/1712.04028"
      github:   "http://github.com/dsrim/dinterp"
      url:      "https://epubs.siam.org/doi/abs/10.1137/18M1168315"
      doi:      "https://doi.org/10.1137/18M1168315"
      year:     "2018"


    - title:    "Imaging of isotropic and anisotropic conductivities from power                  densities in three dimensions" 
      author:   "F. Monard and D. Rim"
      journal:  "Inverse Probl."
      doi:      "https://doi.org/10.1088/1361-6420/aabe5a"
      url:      "http://iopscience.iop.org/article/10.1088/1361-6420/aabe5a/meta"
      arxiv:    "http://arxiv.org/abs/1711.03137"
      github:   "http://github.com/dsrim/powerdensity3d"
      numbers:  "**34** (7), 075005"
      year:     "2018"

    - title:    "Transport reversal for model reduction of hyperbolic
                partial differential equations" 
      author:   "D. Rim, S. Moe, and R. J. LeVeque"
      journal:  "SIAM/ASA J. Uncertainty Quantification"
      year:    "2018"
      doi:     "https://doi.org/10.1137/17M1113679"
      url:     "http://epubs.siam.org/doi/abs/10.1137/17M1113679"
      numbers: "**6** (1), 118-150"
      arxiv:   "https://arxiv.org/abs/1701.07529"

    - title:   "An elementary proof that symplectic matrices have determinant one"
      author:  "D. Rim"
      journal: "Adv. Dyn. Syst. Appl."
      year:    "2017"
      url:   "http://arxiv.org/abs/1505.04240" 
      arxiv:   "http://arxiv.org/abs/1505.04240" 
      numbers: "**12** (1), 15-20"


    - title:   "Generating random earthquake events for probabilistic tsunami hazard assessment (PTHA)"
      author:  "R. J. LeVeque, K. Waagan, F. I. Gonzalez, D. Rim, and G. Lin"
      journal: "Pure Appl. Geophys."
      year:    "2016"
      doi:     "http://dx.doi.org/10.1007/s00024-016-1357-1"
      url:     "http://link.springer.com/article/10.1007%2Fs00024-016-1357-1"
      arxiv:   "https://arxiv.org/abs/1605.02863"
      numbers: "173: 3671"

    - title:    "Explicit error estimates for Courant, Crouzeix-Raviart and Raviart-Thomas finite element methods"
      author:   "C. Carstensen, J. Gedicke, and D. Rim"
      journal:  "J. Comput. Math."
      numbers:  "**30** no. 4, 337-353"
      year:     "2012"
      url:    "https://opus4.kobv.de/opus4-matheon/frontdoor/index/index/docId/931"
      doi:      "https://doi.org/10.4208/jcm.1108-m3677"
      preprint:    "https://opus4.kobv.de/opus4-matheon/frontdoor/index/index/docId/931"


---

{% include image.html url="images/face.jpg" caption="" width="300px" align="right" %}
### About

I am a Postdoctoral Associate at the [Courant Institute], working with
[Benjamin Peherstorfer]. 

Previously, I was a Chu Assistant Professor at [Columbia University]. I
received a PhD in applied math from the [University of Washington], advised by
[Randall J. LeVeque] and [Gunther Uhlmann]. 

[[CV], updated 2019/07/01].

### Research Interests

My interests are in the numerical analysis of partial differential equations
(PDEs) and inverse problems

* Model reduction of parametrized nonlinear hyperbolic systems of conservation
laws for uncertainty quantification (UQ) problems 
* Approximate discrete Radon transform (ADRT) and its applications: Dimensional
splitting, nonlinear dimensionality reduction
* Applications in geophysics and medical imaging: probabilistic tsunami hazard
assessment, storm surge prediction, coupled-physics imaging

### Publications / Preprints / Software

{% for pub in page.pubs %}
{% if pub.image %}
{% include image.html url=pub.image caption="" height="100px" align=thumbnail %}
{% endif %}
{% if pub.url %}[**{{pub.title}}**]({{pub.url}}){% else %}
{% if pub.arxiv %}[**{{pub.title}}**]({{pub.arxiv}}){% else %}
{% if pub.preprint %}[**{{pub.title}}**]({{pub.preprint}}){% else %}
**{{pub.title}}**{% else %}{% endif %}{% endif %}{% endif %}<br />
{{pub.author}}<br />
*{{pub.journal}}*
{% if pub.note %} *({{pub.note}})*
{% endif %} {% if pub.numbers %}{{pub.numbers}}{% endif %} ({{pub.year}}) |  {% if pub.doi %}[[doi]({{pub.doi}})]{% endif %}{% if pub.arxiv %}[[arXiv]({{pub.arxiv}})]{% endif %}{% if pub.preprint %}[[Preprint]({{pub.preprint}})]{% endif %}{% if pub.github %}[[github]({{pub.github}})]{% endif %}
{% if pub.media %}<br />Media: {% for article in pub.media %}[[{{article.name}}]({{article.url}})]{% endfor %}{% endif %}

{% endfor %}

### More Numerical Software

For a full list of relevant numerical softwares, 
please visit my [github page]. <br >
See also:
[*Top ten reasons to not share your code (and why you should anyway)*](https://sinews.siam.org/Details-Page/top-ten-reasons-to-not-share-your-code-and-why-you-should-anyway).

### Contact
<sub>Email: [dr1653@nyu.edu]</sub>

[Benjamin Peherstorfer]: https://cims.nyu.edu/~pehersto
[Courant Institute]: https://cims.nyu.edu/
[Randall J. LeVeque]: http://faculty.washington.edu/rjl/
[Gunther Uhlmann]: http://www.math.washington.edu/~gunther/
[CV]: files/Donsub_Rim_CV.pdf
[dr1653@nyu.edu]: mailto:dr1653@nyu.edu
[github page]: http://github.com/dsrim/
[Columbia University]:http://apam.columbia.edu
[University of Washington]:http://amath.washington.edu
