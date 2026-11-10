---
layout: about
title: About
permalink: /
subtitle: Postdoctoral Researcher, <a href="https://www.chemistry.utoronto.ca/">Department of Chemistry</a>, University of Toronto

profile:
  align: right
  image: seongmin-kim-profile.jpg
  image_circular: false # rounded rectangle; a circle would cut the photo down to a face crop
  more_info: # left empty; the office address lives in the CV contact block

selected_papers: false # the full list lives on the publications page; no need to repeat it here
social: true # icon row at the bottom of the page

announcements:
  enabled: true # news items from the `_news` folder
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

I develop machine learning and large language model methods for designing synthesizable inorganic materials and planning how to make them. I am a postdoctoral researcher in [The Matter Lab](https://www.matter.toronto.edu/) at the University of Toronto, led by [Prof. Alán Aspuru-Guzik](https://scholar.google.com/citations?user=Ag_6KEgAAAAJ).

I received my Ph.D. in Chemical and Biomolecular Engineering from KAIST, working on AI for material synthesis with [Prof. Yousung Jung](https://scholar.google.com/citations?user=y8D-JCAAAAAJ), and continued as a postdoc in his group at Seoul National University. Before that, I studied lithium-ion battery materials for my M.S. at Seoul National University with [Prof. Kyu Tae Lee](https://scholar.google.com/citations?user=L1aEb58AAAAJ), and received my B.S. in Chemical Engineering from POSTECH.

<section class="home-research" aria-label="Research">
{% include research-overview.liquid %}
</section>

<section class="feature" aria-labelledby="materealize-title">
  <p class="feature-eyebrow">Featured project</p>
  <h2 id="materealize-title">Materealize<span class="feature-tagline">: an end-to-end workflow from materials design to materials realization</span></h2>
  <p class="feature-lede">
    Materealize takes a target property as a prompt and carries it all the way to a synthesis report. It generates candidate structures,
    checks their properties and novelty, predicts which ones can actually be made, and proposes how to make them.
  </p>

  <figure class="feature-figure">
    <img
      src="{{ '/assets/img/materealize_steps.gif' | relative_url }}"
      width="2460"
      height="1008"
      loading="lazy"
      decoding="async"
      alt="A user asks to design new inorganic materials with a bandgap around 1.34 eV. Materealize answers in four steps: material generation, property evaluation, synthesizability evaluation, and synthesis planning."
    >
    <figcaption>From a generated material to a plan for making it.</figcaption>
  </figure>

  <div class="feature-modes">
    <div class="feature-mode">
      <h3>Instant mode <span class="feature-time">~2 min</span></h3>
      <p>
        Conditional generation, synthesizability prediction and synthesis planning in one pass: precursors, heating temperature, an explanation of
        the prediction, and a redesigned structure when a candidate is not synthesizable.
      </p>
    </div>
    <div class="feature-mode">
      <h3>Thinking mode <span class="feature-time">~30 min</span></h3>
      <p>
        A selected candidate goes to a multi-agent debate. Specialist agents argue the synthesis route with their own ML tools, and a judge agent
        writes the final synthesis report.
      </p>
    </div>
  </div>

  <div class="feature-split">
    <figure class="feature-figure">
      <img
        src="{{ '/assets/img/multi_agent_debate.gif' | relative_url }}"
        width="892"
        height="908"
        loading="lazy"
        decoding="async"
        alt="Animation of four specialist agents taking turns in a multi-agent debate, with a judge agent receiving the outcome."
      >
      <figcaption>Four specialist agents argue it out; a judge agent finalizes the route.</figcaption>
    </figure>
    <div class="feature-split-text">
      <h3>Multi-agent debate</h3>
      <p>Instead of one model giving one answer, four agents each look at the candidate from a different angle and challenge one another:</p>
      <ul class="feature-agents">
        <li><strong>Precursor agent</strong> on which starting materials to use</li>
        <li><strong>Thermodynamic agent</strong> on whether the target is stable to form</li>
        <li><strong>Surface &amp; kinetics agent</strong> on how the reaction proceeds</li>
        <li><strong>Literature agent</strong> on what has been reported before</li>
      </ul>
      <p>A <strong>judge agent</strong> weighs the debate and returns a synthesis report with the proposed route and the reasoning behind it.</p>
      <p class="feature-links">
        <a href="https://arxiv.org/abs/2601.15743">Read the preprint <i class="fa-solid fa-arrow-up-right-from-square" aria-hidden="true"></i></a>
      </p>
    </div>
  </div>
</section>
