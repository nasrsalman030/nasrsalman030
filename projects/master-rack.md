# Master / RACK

**Product family:** Aetheria · **Domain:** Music

**A modular audio-mastering project for techno and electronic music.**

[Back to the portfolio](../README.md)

## The idea

Mastering tools should make important processing decisions understandable and editable. Master, documented under the working name RACK, starts with manual digital signal processing rather than treating AI as a prerequisite for a useful product.

## The documented architecture

The project describes a C++ processing core, a Web Audio and WebAssembly path, and a Tauri desktop shell. Its modular design is intended to separate processing modules from the interface that controls them.

The documented focus includes low-frequency control, equalization, limiting and different output targets. Browser and native processing are compared within defined numerical tolerances rather than advertised as automatically bit-identical across platforms.

## Engineering focus

Real-time processing must remain predictable. The project's documented constraints exclude blocking work from the audio-processing path and reserve an optional future AI layer for a separate execution boundary.

Listening evaluations and measurements are part of the development method. This overview does not claim that the project outperforms a commercial mastering product or that a listening study has established superiority.

## Development boundary

Manual DSP is the documented first version. The AI co-pilot is a deferred, optional direction. Current platform compatibility, release readiness and measured audio quality have not been independently verified for this portfolio review.

Master / RACK belongs to Aetheria Music, a sibling domain of the self-contained Aetheria Studio system. This portfolio classification does not rename the application or merge codebases. No copyrighted audio examples are included.
