# embedding-ring-visualization
Visualize image embeddings of a rotating 3d model.

A virtual camera orbits a 3D object and renders one frame per step. Each frame is embedded by a pretrained vision encoder (CLIP, SigLIP, DINOv2, ViT, MobileViT) directly in the browser with [transformers.js](https://github.com/huggingface/transformers.js), on WebGPU or WASM. The embeddings are projected to 3D with PCA and with a sinusoidal (ellipse) fit. If the encoder represents the viewpoint smoothly, the frames trace a ring.

Open `index.html` via any static file server (e.g. `python3 -m http.server`). No build step.
