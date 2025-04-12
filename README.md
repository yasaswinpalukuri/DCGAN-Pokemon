# DCGAN-Pokemon
This repository shows battle two architecturally different DCGANs to generate realistic images

As a data scientist passionate about generative AI, I dove into a fun yet challenging project: using Deep Convolutional GANs (DCGANs) to create Pokémon-style images. This wasn’t just about making cool visuals—it was about pushing AI to mimic reality and proving it with data. Here’s how I built, optimized, and evaluated two DCGAN models, delivering insights that recruiters might find compelling.

🎯 My Objective
I aimed to generate Pokémon-style images that could rival the real thing, while rigorously quantifying their quality. Beyond pretty pictures, I asked:

"Can I make AI outputs indistinguishable from reality, and how do I prove it?"

To answer, I designed a pipeline using:

✅ Fréchet Inception Distance (FID): To measure image realism and diversity.

✅ Real-vs-Fake Classifier: To test how well my models fooled a CNN.

This project showcases my ability to blend creativity with analytical rigor—a skill I bring to every machine learning challenge.

🗃️ The Toolkit
Dataset: 819 Pokémon images from Kaggle (128×128 resolution).
Tech Stack: TensorFlow 2.x, Keras, InceptionV3, Matplotlib, leveraging Kaggle’s GPU for efficiency.
Training: Two DCGAN models, each trained for 100 epochs.
My proficiency with these tools reflects my hands-on experience in building and scaling deep learning workflows.

🧱 Designing the Models
I engineered two DCGAN architectures to compare their performance, demonstrating my ability to iterate and optimize:

🔹 Standard DCGAN
    Generator: Dense layer → Reshape → 3 Conv2DTranspose layers → tanh output.
    Discriminator: 2 Conv2D layers → sigmoid.
A lean baseline, prioritizing simplicity to establish a performance floor.
🔸 Custom DCGAN
    Generator: 4 Conv2DTranspose layers with Instance Normalization and 30% Dropout.
    Discriminator: 5 Conv2D layers with Dropout for robustness.
  
Designed to maximize diversity and minimize mode collapse, showing my focus on model stability.
This experimentation highlights my knack for balancing complexity with performance, a critical skill in production-grade AI.

📈 Evaluating Impact
I measured success with two metrics, ensuring a comprehensive assessment:

✅ FID Score

Computed every 10 epochs using 500 real and 500 generated images.
Lower FID = closer alignment to real Pokémon in feature space.
✅ Real-vs-Fake Classifier

A CNN trained to spot fakes. Low accuracy means my generator succeeded in deception.
This dual-metric approach underscores my commitment to robust evaluation, ensuring models don’t just look good—they perform.

📊 Results That Deliver
🔁 FID Performance

Standard DCGAN: Started at 424.8, settled at 388.8—solid but uneven.
Custom DCGAN: Dropped from 424.8 to 296.5, proving superior realism and diversity.
👀 Visual Impact

I generated comparison grids every 10 epochs (real vs. Standard vs. Custom). The Custom DCGAN produced vibrant, detailed images that increasingly mirrored real Pokémon—demonstrating my ability to translate code into tangible outcomes.

🔍 Classifier Insights

Both models achieved 0% classifier accuracy, suggesting they fooled the CNN completely. However, this raised a red flag—likely a data labeling error or overfitting in the classifier. I’m investigating to ensure robustness, reflecting my proactive approach to debugging.
These results showcase my ability to deliver measurable improvements and critically assess my work.

🔑 Skills Demonstrated
Technical Expertise: Mastered GAN architectures, TensorFlow, and GPU-accelerated training.
Problem-Solving: Optimized models with Dropout and Instance Normalization to tackle mode collapse.
Analytical Thinking: Combined FID and classifier metrics for a holistic evaluation.
Transparency: Identified and flagged potential issues (classifier accuracy), prioritizing integrity.
Passion: Turned a fun idea into a rigorous AI experiment, showing my drive to innovate.
🔮 What’s Next for Me?
I’m excited to push generative AI further:

Explore StyleGAN2 or Diffusion Models for photorealistic outputs.
Integrate text-to-image prompts (e.g., “Ice-type Pokémon”) for targeted generation.
Apply GANs to game design or other creative AI use cases.
Join a team where I can scale cutting-edge ML solutions.
🙌 Why This Matters
This project wasn’t just about Pokémon—it was about proving I can take complex AI concepts, build production-ready models, and deliver results that stand up to scrutiny. For recruiters, it’s evidence of my technical depth, creative problem-solving, and passion for machine learning.

🤝 Gratitude
A huge thank you to my talented teammates—Jharana Adhikari, Raemil Corniel, and Uma Maheshwari—for their collaboration and insights. Special gratitude to our professor, Vahid Hadavi, for guiding us through this journey. I’m thrilled with our progress and eager to keep innovating in AI and NLP!

📬 I’m open to opportunities! If you’re hiring data scientists or AI engineers who thrive on innovation, let’s connect. I’d love to discuss how I can contribute to your team—or just chat about GANs over coffee.
