# Improve-Inference-Speed-by-10x-on-GPT-style-TTS-Model
We're looking to improve inference speed by 5-20x on an open-source TTS model called Bark built on a GPT architecture.  Project Description: The Bark TTS model is a GPT style model, taking inspiration from Andre Karpathy's NanoGPT.


We're looking to improve inference speed by 5-20x on an open-source TTS model called Bark built on a GPT architecture.

Project Description:
The Bark TTS model is a GPT style model, taking inspiration from Andre Karpathy's NanoGPT.

Here is a sample of the current audio quality it generates: https://drive.google.com/file/d/1sGZACJrcnY1x9IPoszP97MLmrPTY8mv9/view?usp=sharing

It's already undergone significant improvements, achieving a 1:1 ratio in terms of audio generation time (e.g., 15 seconds of audio takes 15 seconds to generate). Our goal is to further reduce the inference time and implement a streaming mode for real-time audio delivery.

We want the model to start returning audio as soon as the first bit is ready, aiming to deliver the initial audio output in under 1 second, regardless of the total generation time. We are open to using high-performance GPUs or TPUs or other resources to achieve these results.

A few ideas we have on how to optimize so far:

implement TPUs and JAX like was done in this implementation of whisper JAX: https://github.com/sanchit-gandhi/whisper-jax
implement tensorrt
There are likely a lot of ways the model can be made to inference faster, these are just some of the ideas we have so far.

Responsibilities:

Analyze and optimize the existing Bark TTS model for faster inference speed
Implement a streaming mode to enable real-time audio delivery
Test and validate the optimized model and streaming functionality
Key Deliverables:

An optimized Bark TTS model with significantly reduced inference time without sacrificing audio quality
A functional streaming mode that returns the first bit of audio in under 1 second
Documentation of changes and optimizations made to the model
