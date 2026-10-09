## Hi, I'm Hugo

Engineering student at ENSTA Paris, working on **3D computer vision** — turning
ordinary video into geometry you can actually measure.

**Looking for a research or R&D internship** in computer vision, 3D
reconstruction, or learning for robotics.

---

### Featured — Markerless footfall capture from a single phone camera

[![Spider walking, with its footfalls reconstructed in 3D](https://raw.githubusercontent.com/hugodush55/3d-spider-motion-reconstruction/main/figures/contacts.jpg)](https://github.com/hugodush55/3d-spider-motion-reconstruction)

Where does a spider actually put its feet? Measured from handheld phone video,
with no markers and no motion-capture rig.

A walking animal deforms between viewpoints, so it cannot be triangulated. The
ground it walks on cannot. So the pipeline reconstructs the **scene** instead of
the animal — which makes a planted foot *exactly* determined, as the
intersection of its optical ray with the reconstructed ground plane.

- COLMAP sparse SfM with the animal masked out · SAM2 segmentation · geodesic
  morphology for appendage tips · robust plane fitting
- 26 takes, 2 species, 10 577 frames — second species runs through **unmodified**
- 0 identity errors over 712 frame transitions; 131 footfalls extracted
- Every claim backed by a control designed to fail; eight hypotheses refuted
  and documented

**→ [See the project](https://github.com/hugodush55/3d-spider-motion-reconstruction)** · animated demo
and full method inside

---

### Also here

**[voice-emotion-cnn](https://github.com/hugodush55/voice-emotion-cnn)** — speech
emotion recognition from log-mel spectrograms, built so the evaluation actually
means something: splits are by **speaker**, with 5-fold leave-speakers-out
cross-validation, and the CNN trained from scratch is compared against frozen
and fine-tuned ResNet-18 and CNN14 baselines.

**73 % UAR on unseen speakers**, against 16.7 % chance and **42.9 % for human
listeners** on the same audio. Deployed as a Gradio app.

---

### Stack

Python · PyTorch · OpenCV · COLMAP / pycolmap · SAM2 · NumPy / SciPy · Open3D

### Reach me

**[LinkedIn — Hugo Lequy](https://www.linkedin.com/in/hugo-lequy-8b5542310)** ·
open to research and R&D internships.
