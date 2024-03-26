---
title: Adaptive Voice
summary:  Cognitively Adaptive Voice Interface for Driving Assistance
tags:
  - Predict
date: '2024-03-26T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  #caption: Photo by rawpixel on Unsplash
  focal_point: Smart

links:
  #- icon: twitter
  #  icon_pack: fab
  #  name: Follow
  #  url: https://twitter.com/georgecushen
#url_code: ''
url_pdf: 'https://doi.org/10.1145/3613904.3642876'
#url_slides: ''
url_video: 'https://drive.google.com/file/d/1WjKUx6KjPTa81uBeglH_NZydaZc_oGki/view?usp=sharing'

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
#slides: example
---
<div style="text-align: justify;">
  <p>
  Voice assistants have become popular and valuable for drivers driving through complex and unfamiliar road networks. According to a recent report, the number of adults in the US that have used a voice assistant in their cars rose to 129.7 million in
  2020, with 83.8 million monthly users and 29.7 million daily users. Drivers follow instructions (e.g., on where to make a turn) and acquire information (e.g., of the real-time traffic) from voice assistants. Current systems play voice messages in a predefined manner, with fixed content, and at a fixed speed. However, as drivers may encounter different events while driving, which can induce different levels of cognitive load, they may have diverse capabilities or capacities of consuming the information from voice assistants and following their instructions. As a result, the same message can be overwhelming to a driver with a heavy cognitive load (e.g., during an emergency), while more details can be appreciated when the car is at a stop.
  </p>

  <p>
  To address this issue, we propose AdaptiveVoice, which presents voice instructions in an adaptive manner. AdaptiveVoice estimates the cognitive load of users and adjusts the level of details, speech speed, and repetition to provide sufficient but not overwhelming information to assist their driving. While considering users’ mental inertia of expecting the voice instructions to be in similar formats as the previous, AdaptiveVoice also maintains temporal consistency when possible.
  </p>

  <p>
  Before implementing AdaptiveVoice, we conducted a user study to understand the users’ need for adaptive voice messages when they are at different levels of cognitive load. We apply a dual-task experimental design where the cognitive load of a primary task is affected by the difficulty of a secondary task happening at the same time, i.e., the more difficult the secondary task is, the higher cognitive load users would perceive in the primary task. The primary task is following the voice instructions as the task of interest, and the secondary task is designed to be about memorizing an array of numbers. The selected secondary task requires the user to memorize and compare the digits, creating additional mental loads. We control the task difficulty by the length of the array and the number of digits to memorize. In the primary task, we test voice instructions with five levels of details, three speech speeds, and in the conditions of with or without repetition. Results from twelve participants show that the presentation of voice messages significantly affects users’ reaction time and accuracy in following the instructions. The participants prefer different formats of voice instructions with different levels of cognitive load, and this verifies the need for adaptation.
  </p>
  <p>
  Based on the findings and data obtained in the first study, we built an algorithm to optimize the presentation of voice instructions, taking as input the user’s cognitive load and previous presentation formats. The algorithm is prioritized to present instructions close to the preferred formats of users at the corresponding level of cognitive load and similar to the previous instructions recorded in the interaction history.
  </p>
  <p>
  We add HUD as a control variable, as it becomes a common setup in modern vehicles. To be noted, the effects of HUD on driving performance have been studied by previous research, and that is not our main focus of the study. We use HUD only to investigate the impacts of adaptive voice interfaces in broader usage scenarios. Results indicate that users benefit from AdaptiveVoice with reduced response time and improved driving performance, particularly when their driving is augmented with HUD. In addition, participants’ subjective ratings and comments support the objective results and confirm their inclination to the use of adaptation for voice messages.
  </p>
  <p>
  In summary, we make the following contributions:
  <ul>
      <li>We introduced AdaptiveVoice, an advanced system designed to estimate users’ cognitive load and adapt the voice instruction presentation of driving assistants in real time. This system provides tailored assistance to drivers, ensuring the voice instructions are sufficient and not overwhelming, thereby optimizing user experience and comprehension.</li>
      <li>We quantified the effects of different voice instruction formats on users’ task performance while following instructions under varying levels of cognitive load. The study results allow us to extract and understand drivers’ preferences for voice instruction presentation.</li>
      <li>We assessed the efficacy of AdaptiveVoice through a simulated driving task, comparing it with a fixed-format baseline in a virtual driving environment. This evaluation demonstrates AdaptiveVoice’s ability to significantly reduce response times and improve driving performance, indicating its practical feasibility and effectiveness in real-world driving scenarios.</li>
  </ul>
  </p>
