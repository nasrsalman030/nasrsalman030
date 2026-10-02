# Aetheria Studio

**Product family:** Aetheria · **Domain:** Studio

**A workspace for AI-assisted website creation and creative workflows.**

[Back to the portfolio](../README.md)

## The problem

Website work often moves between references, layout decisions, generated content and separate tools. Aetheria Studio is intended to make that process easier to navigate without hiding the components that perform the work.

## The documented approach

The project documentation describes a Next.js workspace over a website-generation engine, a Python processing pipeline and an inference service. Those boundaries keep the interface separate from generation and processing.

Three creation modes are described: **Clone** turns a reference into an editable starting point; **Composer** combines sections and visual elements; **Wizard** starts from a structured brief. A shared template contract connects the workflows. References and assets still require appropriate rights and permissions.

The broader creative direction includes interface design, effects and knowledge enrichment. Retrieval and an improving knowledge store are distinct from training a new production model; they should not be presented as the same achievement.

Aetheria Studio is a self-contained product system. Its internal tools and component repositories stay within that system. Aetheria Music is a sibling domain, not an extension inserted into the Studio.

## Engineering focus

The important design questions are how tools exchange a consistent artifact, how the interface explains unavailable services, and how proposed changes remain inspectable. A shared workspace does not require merging all engines into one application.

## Development boundary

The reviewed documentation describes the shell and creation modes as implemented, while parts of Media Forge remain in development and model-training work remains research. This page does not claim that a fresh build or end-to-end runtime was verified for this portfolio review.

Documentation reviewed: **1 October 2026**. Source code, runtime configuration and private creative material are not included in this overview.
