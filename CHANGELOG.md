# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2025-11-18

### Initial Release

#### Features
- **HYPIR Image Restoration Node**: ComfyUI custom node for image restoration using HYPIR LoRA on Stable Diffusion 2.1
- **Flexible Upscaling**: Support for 1-8× upscale factors with configurable scaling modes (factor or longest side)
- **Tiled VAE Processing**: Efficient processing of high-resolution images with configurable patch size and stride
- **LM Studio Integration**: Optional prompt enhancement through OpenAI-compatible LM Studio endpoint
- **Restoration Controls**: 
  - Enhancement strength blending
  - Detail boost with unsharp-mask style enhancement
  - Configurable detail sigma for fine-tuning
- **Dual Licensing**: Non-commercial (CC BY-NC 4.0) and commercial licensing options

#### Installation Methods
- ComfyUI Manager support for one-click installation
- Manual git clone installation
- Registered in ComfyUI Manager custom node list

#### Documentation
- Comprehensive README with installation instructions
- Quick start guide
- LM Studio configuration guide
- Example workflow screenshot
- Comparison images showing restoration quality
- Troubleshooting section

#### Technical Implementation
- Custom model folder registration (`hyper_hypir`)
- Automatic model directory creation
- Support for SD 2.1 base (512px) and full (768px) models
- Memory-efficient tiled decoding for large images
- Configurable seed for reproducible results

#### Dependencies
- ComfyUI compatible
- PyTorch, Diffusers, Transformers, PEFT, Accelerate
- Optional: requests (for LM Studio integration)

[1.0.0]: https://github.com/EricRollei/HYPIR-ComfyUI/releases/tag/v1.0.0
