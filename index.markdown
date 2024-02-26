---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: ""
---

I work on the foundations of quantum information theory and its scientific applications. My research interests include
- Quantum Shannon theory, quantum error correction and fault-tolerant quantum computing
- Computational number theory, algebraic geometry and the arithmetic of quantum circuits
- Algorithms, optimization and computational complexity theory
- Quantum field theory and mathematical physics
- Machine learning theory and applications

## Select publications

{% for paper in site.papers -%}
- {% if paper.journal != "" %}[{{paper.title}}]({{paper.journal}}) {% else %} {{paper.title}} {% endif %} - [![arXiv](/png/arXiv.png){:width="12px" height=12px"}](https://arxiv.org/abs/{{paper.arxiv}})
{% endfor %}