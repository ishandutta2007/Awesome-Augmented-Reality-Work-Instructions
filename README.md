# Awesome-Augmented-Reality-Work-Instructions

# Awesome-Augmented-Reality-Work-Instructions



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on AR Step-by-Step Guidance, In-Situ Authoring & Procedural Training*

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Augmented Reality Work Instructions**. These tools help frontline workers perform complex assembly, maintenance, and inspection tasks with step-by-step AR guidance overlaid directly on physical equipment.



**Examples** include Microsoft Dynamics 365 Guides, PTC Vuforia Expert Capture, Taqtile Manifest, Atheer, Scope AR WorkLink, TeamViewer Frontline, Proceedix, RE'FLEKT, CareAR, and HoloBuilder (the category leaders).



**Open-source emphasis**: The open-source ecosystem for AR work instructions is **emerging and research-focused**. **MirageXR** (Community Edition) is the standout—a reference implementation of an XR training system validated in Horizon 2020 projects with over 550 participants across medicine, aviation, and space . **TrainAR** provides a holistic AR authoring tool for non-programmers with visual scripting and didactic frameworks . **Microsoft SIGMA** is an open-source research platform for situated interactive guidance on HoloLens 2 . **Tuto-AR** demonstrates Flutter-based AR tutorials using ARCore and ML Kit. This section documents these focused solutions honestly.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents



- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Microsoft Dynamics 365 Guides](https://learn.microsoft.com/en-us/dynamics365/mixed-reality/guides/)**  

  **Enterprise AR work instruction platform for HoloLens 2.** Provides step-by-step holographic instructions overlaid on real equipment, with in-situ authoring, 3D models, photos, videos, and annotations. **Critical lifecycle notice**: **End of support December 31, 2026** . Subscriptions may be purchased or renewed until **November 1, 2025**. After that date, no security updates, bug fixes, or technical support.



- **[PTC Vuforia Expert Capture](https://www.ptc.com/en/products/vuforia/expert-capture)**  

  **AR work instruction creation and delivery platform.** Captures expert procedures via RealWear or mobile devices, then delivers AR-guided instructions to frontline workers. **Note**: **Vuforia Vantage on RealWear ends support December 1, 2026** .



- **[Taqtile Manifest](https://www.taqtile.com/)**  

  **AR/MR work instruction platform for complex operations.** Enables subject matter experts to capture and digitally document procedures non-technically—in nearly the same time it takes to perform the job, they can author a procedure that thousands can follow . Supports **HoloLens 2, Magic Leap, RealWear, iPads, Android, and Chrome**. **Deployment**: Public cloud, private cloud, or **air-gapped on-premises** with no internet connection . Used in manufacturing, defense, transportation, pharmaceutical, and utilities .



- **[Atheer](https://www.atheerair.com/)**  

  **AR work instruction and remote assistance platform.** Provides AR-powered work instructions created without coding, secure chat for peer/expert collaboration, and multi-party remote video assistance.



- **[Scope AR WorkLink](https://www.scopear.com/)**  

  **AR work instruction authoring and delivery.** **WorkLink Scenarios** support 3D work instructions with AR mode, active tracking, and overlay modes for equipment in front of the worker or standalone 3D rendering .



- **[TeamViewer Frontline](https://www.teamviewer.com/en/products/frontline/)**  

  **Enterprise AR platform for frontline workers with vision picking, assembly, and remote assistance.** **Proven at scale**: DHL Supply Chain at 25 sites with 1,500 employees daily (15% productivity increase); Coca-Cola HBC at 35 warehouses in 17 countries (99.99% picking accuracy) . Supports mobile devices and smart glasses.



- **[Proceedix](https://www.proceedix.com/)**  

  **Connected worker platform with AR work instructions and inspections.** Provides step-by-step digital work instructions, remote assistance, and inspection workflows.



- **[RE'FLEKT](https://www.reflekt.com/)**  

  **AR work instruction and remote support platform.** Provides AR-guided procedures, remote expert assistance, and content authoring.



- **[CareAR](https://www.carear.com/)**  

  **AR platform for service and operations with work instructions and remote assistance.** Provides step-by-step AR guidance, measurement tools, and session recording.



- **[HoloBuilder](https://www.holobuilder.com/)**  

  **360° reality capture and AR work instruction platform.** Provides construction progress documentation and AR-guided field operations.



## Open-Source GitHub Projects



### Full XR Training Platforms



- **[MirageXR (Community Edition)](https://github.com/WEKIT-ECS/MIRAGE-XR)**

  **The most mature open-source XR training system for complex work environments.** **Community Edition** is the B2B open-source reference implementation offered "as is" for the XR developer community . **Key features**: **In-situ authoring and experience capture** — create content directly in XR, reducing production time; **Ghost tracks** — holographic representation of expert performance (body position, gaze, gestures, voice) embedded in the physical workplace; **Experiential learning** — trainees follow a sequence, review their performance, and repeat; **Open standards** — implements **IEEE P1589-2020** for AR learning experience models; **IEEE xAPI** integration for performance analysis . **Validation**: Based on Horizon 2020 project WEKIT results, validated with **over 550 participants** in pilot trials across **medicine, aviation, and space** . **Best for**: Organizations and researchers building custom XR training systems for complex procedural tasks.



### AR Authoring Tools for Non-Programmers



- **[TrainAR](https://github.com/jan-behrends/TrainAR-1)**

  **Open-source AR authoring tool for procedural training on handheld Android and iOS devices.** **Unity 2022.1 Editor Extension** . **Key features**: **Visual scripting stateflow** inspired by work-process-analyses — authors import 3D models, convert them to TrainAR objects, and reference them in a stateflow to create procedural flows of instructions, user actions, and feedback; **Onboarding animations**, tracking solutions, assembly placements, layered feedback modalities, and training assessments out of the box; **No AR-specific expertise required** . **Deployment**: Deploy to Android and iOS from Unity Windows/macOS/Linux Editor. **Best for**: Non-programmers and programmers without AR expertise wanting to create interactive procedural AR trainings.



### Research Platforms



- **[Microsoft SIGMA](https://github.com/microsoft/SIGMA)**

  **Open-source research platform for situated interactive guidance on HoloLens 2.** **Key features**: **Step-by-step task guidance** with language and vision models; **Dynamic task generation** — tasks can be pre-defined or generated on the fly; **Object detection and highlighting** using vision models like **Detic** and **SEEM**; **Question answering** — answer user queries during task execution . **Architecture**: Client-server — data streams from HoloLens 2 processed on desktop server, bypassing device limitations . Built on **Platform for Situated Intelligence** framework. **Best for**: Researchers wanting to leapfrog basic engineering challenges of full-stack interactive AR applications.



### Handheld AR Tutorials



- **[Tuto-AR](https://github.com/erico-ke/TUTO-AR.-HackReality-Hackaton)**

  **Flutter-based AR tutorial application with object recognition.** **Key features**: **ARCore** for mixing physical and digital worlds; **ML Kit** for object recognition in the physical world to identify tutorial-relevant objects; **Real-time step visualization** — users see tutorial steps overlaid on real objects (e.g., changing car oil, installing RAM) . **Tech stack**: Flutter, Dart, ARCore, ML Kit . **Status**: Hackathon project (HackReality 2024) — early-stage but demonstrates the concept. **Best for**: Developers exploring handheld AR tutorials with object recognition.



### Additional Strong Open-Source Options



- **Full XR Training**: **MirageXR** (IEEE P1589-2020, ghost tracks, validated in medicine/aviation/space) .

- **AR Authoring**: **TrainAR** (visual scripting, no AR expertise needed) .

- **Research**: **Microsoft SIGMA** (HoloLens 2, Detic/SEEM vision models) .

- **Handheld AR**: **Tuto-AR** (Flutter, ARCore, ML Kit) .

- **Note**: The open-source ecosystem lacks production-ready alternatives to enterprise platforms like Dynamics 365 Guides, Vuforia Expert Capture, and Taqtile Manifest.



**Frameworks for building custom systems**: Combine **MirageXR** for a validated XR training foundation with ghost tracks and IEEE standards, **TrainAR** for visual scripting-based AR authoring on handheld devices, **Microsoft SIGMA** for research-grade interactive guidance on HoloLens 2, and **Tuto-AR** for handheld AR tutorials with object recognition. Add **Unity** for AR development and **HoloLens 2** or **Android/iOS** devices for deployment.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- AR work instruction platforms handle sensitive operational and procedural data; ensure proper access controls and compliance with organizational security policies.

- **Critical lifecycle notice**: **Microsoft Dynamics 365 Guides** reaches **end of support December 31, 2026** . Subscriptions may be purchased or renewed until **November 1, 2025**. Users should migrate to alternatives before that date.

- **Open-source reality**: The open-source ecosystem for AR work instructions is **emerging and research-focused**. **MirageXR** is the standout—a validated XR training system with ghost tracks, IEEE P1589-2020 compliance, and pilot trials across medicine, aviation, and space . **TrainAR** provides a non-programmer-friendly authoring tool with visual scripting . **Microsoft SIGMA** offers a research platform for HoloLens 2 with language and vision models . However, **commercial platforms** (Taqtile Manifest, Vuforia Expert Capture, TeamViewer Frontline, Atheer) provide **enterprise-grade deployment, proven scale at companies like DHL and Coca-Cola, and air-gapped security options** that open-source alternatives require significant development to match. The open-source path is best suited for **research, custom application development, or organizations with strong XR engineering capacity**.



---



**Made for industrial engineers, field service technicians, XR developers, and training professionals.**

Let's make AR work instructions more open, accessible, and effective.
