---
title: Compilation-Guided Energy Optimization for ML
template: page
summary: EECS 583 Course Project
cv_pdf: pdf/Dhanvi_Bharadwaj_Resume.pdf
img: images/graph_level.png
importance: 1
category: courses
related_publications:
---

We developed a framework that dynamically balances computation, memory, and network resources at both the graph and operator levels. By strategically overlapping computation and communication, tuning CUDA kernel parameters, and adapting these settings as GPU frequency changes, we achieved up to 23% energy savings in key training stages compared to previous methods-without sacrificing performance. Our results show that energy-optimal configurations often differ from those that minimize execution time, highlighting the need for dynamic, frequency-aware optimization in energy-efficient AI training.

<div style="border: 1px solid #ccc; border-radius: 8px; overflow: hidden; box-shadow: 0 4px 12px rgba(0,0,0,0.1);">
  <iframe 
    src="/pdf/CSE_583_Final_Report.pdf#toolbar=0&navpanes=0&view=FitH  " 
    style="width: 100%; height: 1000px; border: none;" 
    title="EECS 583 Final Report"
  >
    Your browser does not support iframes. 
    <a href="/pdf/CSE_583_Final_Report.pdf" target="_blank">Download the PDF</a> instead.
  </iframe>
</div>
