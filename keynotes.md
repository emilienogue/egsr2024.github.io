---
layout: cvmp-default
title: Keynotes
year: 2024
---

<style>
  /* Add CSS styles to control image width */
  .keynotes-image {
    float: left;
    width: 30%; /* Set the image width to 20% of the container width */
    margin-right: 10px; /* Optional: Add some margin for spacing */
  }

  /* Add CSS styles to clear the float and separate keynotes */
  .keynote-container::after {
    content: "";
    display: table;
    clear: both;
  }
</style>

<div class="keynote-container">
  <!-- First Keynote -->
  <h3>Demystifying peripheral vision</h3>
  <h3><em>Ruth Rosenholtz</em></h3>

  <img class="keynotes-image" src="{{site.url}}/img/keynotes/RosenholtzHeadshot.jpg" alt="Ruth Rosenholtz">
  <strong>Bio</strong>: Ruth Rosenholtz is a Principal Research Scientist at NVIDIA, having recently joined after 20 years in MIT’s Department of Brain & Cognitive Sciences and CSAIL. She joined MIT after 7 years at the Palo Alto Research Center (formerly Xerox PARC). She has a B.S. in Engineering from Swarthmore College, and a Ph.D. from UC Berkeley in EECS. She brings her background in electrical engineering, specifically computer vision, to the study of human vision, including visual search, perceptual organization, visual clutter, and peripheral vision. Her work focuses on developing predictive computational models of visual processing.<br>

  <a href="https://persci.mit.edu/people/rosenholtz">Website</a>

  <strong>Abstract</strong>:Recent advances in human vision research have pointed toward a theory that unifies many aspects of vision. What one can perceive at a glance, i.e. in a single fixation, is of critical importance to the performance of many visual tasks. Perception at a glance, in turn, hinges on the strengths and limitations of peripheral vision. In this talk I will discuss several pervasive myths about peripheral vision, as well as what is actually true: Peripheral vision is dominated not by loss of acuity, but rather by its vulnerability to clutter, known as visual crowding. Nonetheless, despite significant loss of information, humans rely on peripheral vision for a broad range of visual tasks. People may not always point their eyes at objects of interest, because that may not always be optimal for real-world tasks. Rather, we move our eyes as part of a complex tradeoff between the information available in the fovea vs. periphery, and the costs of shifting one’s gaze.


</div>

<hr>

<div class="keynote-container">
  <!-- Second Keynote -->
  <h3>What are Good Representations for Controllable Generative Models</h3>
  <h3><em>Niloy Mitra</em></h3>

  <img class="keynotes-image" src="{{site.url}}/img/keynotes/NiloyMitra.jpeg" alt="Niloy Mitra">
  <strong>Bio</strong>: Niloy J. Mitra leads the Smart Geometry Processing group in the Department of Computer Science at University College London and the Adobe Research London Lab. He received his Ph.D. from Stanford University under the guidance of Leonidas Guibas. His research focuses on developing machine learning frameworks for generative models for high-quality geometric and appearance content for CG applications. He was awarded the Eurographics Outstanding Technical Contributions Award in 2019, the British Computer Society Roger Needham Award in 2015, and the ACM SIGGRAPH Significant New Researcher Award in 2013. He was elected as a fellow of Eurographics in 2021 and served as the Technical Papers Chair for SIGGRAPH in 2022. His work has also earned him a place in the SIGGRAPH Academy in 2023. Besides research, Niloy is an active DIYer and loves reading, cricket, and cooking.<br>

  <a href="https://geometry.cs.ucl.ac.uk">Website</a>
 
  <strong>Abstract</strong>: Foundational models have rapidly emerged as powerful generative models. In the context of content creation workflows, such image generators are currently controlled by domain-specific conditioning signals (e.g., prompts, depth, joint locations). This, however, makes iterative content creation difficult as 'identity' of object(s) can change in unpredictable ways as the user refines the creation. In this talk, I will discuss how classical representations can be meaningfully used to control pretrained generative models to generate and subsequently edit visual content using easy-to-author high-level guidance. I will report on our recent attempts to mix differential geometry and neural networks to build universal algorithms that do not require huge amounts of 3D training data and discuss open challenges ahead. I will discuss applications in image creation, feature extraction, and image editing. 
</div>
