---
title: Enhancing Foveated Rendering with Weighted Reservoir Sampling
authors:
- Ville Cantory
- Darya Biparva
- Haoyu Tan
- Tongyu Nie
- John Schroeder
- Ruofei Du
- Victoria Interrante
- Piotr Didyk
date: '2025-12-01'
publishDate: '2026-07-21T00:00:00Z'
publication_types:
- paper-conference
publication: '*The 18th ACM SIGGRAPH Conference on Motion, Interaction, and Games (MIG ''25)*'
doi: 10.1145/3769047.3769058
tags:
- conference
---
## Abstract
Spatiotemporal sensitivity to high frequency information declines with increased peripheral eccentricity. Foveated rendering exploits this by decreasing the spatial resolution of rendered images in peripheral vision, reducing the rendering cost by omitting high frequency details. As foveation levels increase, the rendering quality is reduced, and traditional foveated rendering systems tend not to preserve samples that were previously rendered at high spatial resolution in previous frames. Additionally, prior research has shown that saccade landing positions are distributed around a target location rather than landing at a single point, and that even during fixations, eyes perform small microsaccades around a fixation point. This creates an opportunity for sampling from temporally neighbouring frames with differing foveal locations to reduce the required rendered size of the foveal region while achieving a higher perceived image quality. We further observe that the temporal presentation of pixels frame-to-frame can be viewed as a data stream, presenting a random sampling problem. Following this intuition, we propose a Weighted Reservoir Sampling technique to efficiently maintain a reservoir of the perceptually relevant high quality pixel samples from previous frames and incorporate them into the computation of the current frame. This allows the renderer to render a smaller region of foveal pixels per frame by temporally reusing pixel samples that are still relevant to reconstruct a higher perceived image quality, while allowing for higher levels of foveation. Our method operates on the output of foveated rendering, and runs in under 1 ms at 4K resolution, making it highly efficient and integrable with real-time VR and AR foveated rendering systems.

