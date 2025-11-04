# BatmanComfyFlow

A collection of ComfyUI workflows for AI image and video generation. This repository contains various pre-configured workflows for different creative tasks, from basic text-to-image generation to advanced video interpolation and animation.

## What is ComfyUI?

ComfyUI is a powerful node-based interface for Stable Diffusion and other AI image/video generation models. These workflow JSON files can be imported directly into ComfyUI to quickly set up complex generation pipelines.

## 🎨 Available Workflows

### Video Generation & Animation

| Workflow | Description | Use Case |
|----------|-------------|----------|
| **SVD_Workflow.json** | Stable Video Diffusion workflow with double refinement | Convert static images into smooth video animations |
| **workflow_image_to_video.json** | Basic image-to-video conversion pipeline | Quick image animation with SVD |
| **workflow_txt_to_img_to_video.json** | Complete text → image → video pipeline | Generate video from text prompts end-to-end |
| **frames_to_video.json** | Compile individual frames into video | Batch process frames into video files |
| **animeinterpolworkflow.json** | Anime-style frame interpolation | Create smooth anime animations |
| **basic_first_last_interpolation.json** | Interpolate between first and last frames | Generate transition animations |

### Image Generation & Enhancement

| Workflow | Description | Use Case |
|----------|-------------|----------|
| **basic_turbo_w_refiner.json** | SDXL Turbo with refiner pipeline | Fast high-quality image generation |
| **Text Lora Olivio workflow.json** | Text generation with LoRA fine-tuning | Custom styled text-to-image with LoRA models |
| **Textual_Inversion_Embeddings_workflow.json** | Textual inversion embeddings integration | Use custom trained embeddings in generation |
| **RTFKT_Workflow.json** | RTFKT-style generation pipeline | Fashion/streetwear oriented generation |

## 🚀 Quick Start

1. **Install ComfyUI**: Follow the [official ComfyUI installation guide](https://github.com/comfyanonymous/ComfyUI)
2. **Download workflows**: Clone this repository or download individual workflow JSON files
3. **Import into ComfyUI**:
   - Open ComfyUI in your browser
   - Click "Load" button
   - Select a workflow JSON file from this repository
4. **Configure & Generate**:
   - Adjust parameters as needed
   - Queue the workflow to start generation

## 📋 Requirements

- ComfyUI installed and running
- Required models downloaded:
  - SDXL base/turbo models (for image generation workflows)
  - SVD models (for video generation workflows)
  - Any LoRA or embedding files referenced in specific workflows
- Sufficient VRAM (most workflows require 8GB+)

## 🖼️ Preview Images

This repository includes example outputs:
- `Comfy-doom.png` - Example doom-style generation
- `a1111-venom.png` - Venom character generation
- `svd-double-refinement.png` - SVD video workflow preview

## 📝 Workflow Details

### Video Workflows

**SVD (Stable Video Diffusion)**: Uses the ImageOnlyCheckpointLoader and SVD conditioning nodes to create smooth video animations from static images. Includes advanced features like CFG guidance and motion control.

**Text-to-Video Pipeline**: Combines SDXL image generation with SVD video diffusion to create videos directly from text prompts. Ideal for rapid prototyping of video concepts.

**Frame Interpolation**: Takes keyframes and generates smooth transitions between them using advanced interpolation techniques. Perfect for animation workflows.

### Image Workflows

**SDXL Turbo + Refiner**: Fast generation using SDXL Turbo models with optional refiner pass for enhanced quality. Optimized for quick iterations.

**LoRA Integration**: Demonstrates how to integrate custom LoRA (Low-Rank Adaptation) models for specialized styles or subjects.

**Textual Inversion**: Shows how to use custom embeddings trained on specific concepts or styles.

## 🛠️ Customization Tips

- **Adjust resolution**: Most workflows support resolution changes, but stay within model limits
- **Tweak CFG scale**: Higher values follow prompts more closely, lower values allow more creativity
- **Frame counts**: Video workflows allow customization of output length
- **Seed control**: Lock seeds for reproducible results
- **Batch processing**: Many workflows support batch generation

## 🤝 Contributing

Contributions welcome! If you have interesting ComfyUI workflows to share:

1. Fork this repository
2. Add your workflow JSON file with a descriptive name
3. Update this README with workflow description
4. Submit a pull request

## 📄 License

This repository is provided as-is for educational and creative purposes. Individual workflows may incorporate various open-source components. Please respect the licenses of underlying models and tools.

## 🔗 Resources

- [ComfyUI GitHub](https://github.com/comfyanonymous/ComfyUI)
- [ComfyUI Examples](https://comfyanonymous.github.io/ComfyUI_examples/)
- [Stable Diffusion](https://stability.ai/)
- [SDXL Documentation](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0)

## ⚠️ Notes

- Large workflow files (>1MB) may take time to load in ComfyUI
- Ensure you have all required custom nodes installed
- Check ComfyUI console for missing dependencies
- Some workflows may require specific checkpoint versions

---

**Created by**: Batman (probably not the real one 🦇)
**Last Updated**: 2024

For questions or issues, please open a GitHub issue.
