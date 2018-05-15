---
layout: page
title: 
permalink: /
pubs:
    - title:    "Model reduction of a parametrized scalar hyperbolic conservation law using displacement interpolation" 
      author:   "D. Rim and K.T Mandli"
      journal:  "In preparation"
      year:     "2018"

    - title:    "Displacement interpolation using monotone rearrangement" 
      author:   "D. Rim and K.T Mandli"
      journal:  "Preprint"
      arxiv:    "https://arxiv.org/abs/1712.04028"
      year:     "2017"

    - title:    "Dimensional splitting of hyperbolic partial differential
                 equations using the Radon transform" 
      author:   "D. Rim"
      journal:  "Preprint."
      arxiv:   "https://arxiv.org/abs/1705.03609"
      year:     "2017"

    - title:    "Imaging of isotropic and anisotropic conductivities from power                  densities in three dimensions" 
      author:   "F. Monard and D. Rim"
      journal:  "Accepted to Inverse Probl."
      arxiv:    "http://arxiv.org/abs/1711.03137"
      github:   "http://github.com/dsrim/powerdensity3d"
      year:     "2017"

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
      journal:  "J. Comput. Math. **30**"
      numbers:  "no. 4, 337-353"
      year:     "2012"
      url:    "https://opus4.kobv.de/opus4-matheon/frontdoor/index/index/docId/931"
      doi:      "https://doi.org/10.4208/jcm.1108-m3677"
      preprint:    "https://opus4.kobv.de/opus4-matheon/frontdoor/index/index/docId/931"


---

{% include image.html url="images/coarsevfine_title.png" caption="" width="400px" align="right" %}
### About

I am a Chu Assistant Professor of Applied Mathematics at [Columbia University].

Previously, I was a PhD student at the [University of Washington],
advised by [Randall J. LeVeque] and [Gunther Uhlmann].


### Research Interests

My interests are in the numerical analysis of 
partial differential equations (PDEs) and inverse problems
* Uncertainty quantification (UQ) concerning nonlinear hyperbolic systems of conservation laws, via reduced order models (ROMs). 
* Target applications are geophysical problems: probabilistic tsunami hazard assessment (PTHA) and statistical tsunami source inversion. 
* Inverse anisotropic conductivity from power densities in dimension three.

### Publications and Preprints

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
{% endif %} (*{{pub.year}}*) 
{% if pub.numbers %}*{{pub.numbers}}*{% endif %} {% if pub.doi %}[[doi]({{pub.doi}})]{% endif %}{% if pub.arxiv %}[[arXiv]({{pub.arxiv}})]{% endif %} {% if pub.preprint %}[[Preprint]({{pub.preprint}})]{% endif %}{% if pub.github %}[[github]({{pub.github}})]{% endif %}
{% if pub.media %}<br />Media: {% for article in pub.media %}[[{{article.name}}]({{article.url}})]{% endfor %}{% endif %}

{% endfor %}

### Numerical Software

For a full list of relevant numerical softwares, 
please visit my [github page]. <br >
See also:
[*Top ten reasons to not share your code (and why you should anyway)*](https://sinews.siam.org/Details-Page/top-ten-reasons-to-not-share-your-code-and-why-you-should-anyway).

### Contact
<sub>500 W. 120th St 200 S.W. Mudd<br />
Mail Code: 4701 <br />
Applied Physics and Applied Mathematics <br />
Columbia University<br />
New York, NY, USA, 10027-6623 <br />
Email: [dr2965@columbia.edu] <br /></sub>

[Randall J. LeVeque]: http://faculty.washington.edu/rjl/
[Gunther Uhlmann]: http://www.math.washington.edu/~gunther/
[dr2965@columbia.edu]: mailto:dr2965@columbia.edu
[github page]: http://github.com/dsrim/
[Columbia University]:http://apam.columbia.edu
[University of Washington]:http://amath.washington.edu
