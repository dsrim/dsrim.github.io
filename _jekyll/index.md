---
layout: page
title: 
permalink: /
pubs:
    - title:    "Transport reversal for model reduction of hyperbolic
                partial differential equations" 
      author:   "D. Rim, S. Moe, and R. J. LeVeque"
      journal:  "Preprint."
      year:     "2016"

    - title:   "Generating random earthquake events for probabilistic tsunami hazard assessment (PTHA)"
      author:  "R. J. LeVeque, K. Waagan, F. I. Gonzalez, D. Rim, and G. Lin"
      journal: "Pure Appl. Geophys."
      year:    "2016"
      doi:     "http://dx.doi.org/10.1007/s00024-016-1357-1"
      url:     "http://link.springer.com/article/10.1007%2Fs00024-016-1357-1"
      arxiv:   "https://arxiv.org/abs/1605.02863"

    - title:   "An elementary proof that symplectic matrices have determinant one"
      author:  "D. Rim"
      journal: "Preprint."
      year:    "2015"
      arxiv:   "http://arxiv.org/abs/1505.04240" 

    - title:    "Explicit error estimates for Courant, Crouzeix-Raviart and Raviart-Thomas finite element methods"
      author:   "C. Carstensen, J. Gedicke, and D. Rim"
      journal:  "J. Comput. Math. **30**"
      numbers:  "no. 4, 337-353"
      year:     "2012"
      url:      "http://123.57.41.99/Jwk_jcm/EN/abstract/abstract9777.shtml"
      preprint:    "https://opus4.kobv.de/opus4-matheon/frontdoor/index/index/docId/931"


---

{% include image.html url="images/coarsevfine_title.png" caption="" width="400px" align="right" %}
### About

I am a PhD Candidate of Applied Mathematics at the University of Washington,
Seattle. <br />
My advisors are [Randall J. LeVeque] and [Gunther Uhlmann].

### Research Interests

My interests are in the Numerical Analysis of 
partial differential equations (PDEs) and inverse problems
* Uncertainty Quantification (UQ) via of nonlinear hyperbolic systems of conservation laws via Reduced Order Models (ROMs). 
* Target applications are geophysical problems: Probabilistic Tsunami Hazard Assessment (PTHA) and statistical tsunami source inversion. 
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
{% if pub.numbers %}*{{pub.numbers}}*{% endif %}{% if pub.doi %}[[doi]({{pub.doi}})]{% endif %}{% if pub.arxiv %}[[arXiv]({{pub.arxiv}})]{% endif %} {% if pub.preprint %}[[Preprint]({{pub.preprint}})]{% endif %}
{% if pub.media %}<br />Media: {% for article in pub.media %}[[{{article.name}}]({{article.url}})]{% endfor %}{% endif %}

{% endfor %}

### Contact

Lewis Hall <br />
Applied Mathematics <br />
University of Washington <br />
Seattle, WA, USA <br />
98195-3725 <br />
Email: [drim@uw.edu]

[Randall J. LeVeque]: http://faculty.washington.edu/rjl/
[Gunther Uhlmann]: http://www.math.washington.edu/~gunther/
[drim@uw.edu]: mailto:drim@uw.edu
