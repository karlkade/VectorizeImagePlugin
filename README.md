# VectorizeImage Plugin for Godot

VectorizeImage is a custom Godot plugin that turns raster textures into triangulated meshes using random distribution and edge detection without segmentation or with segmentation. Perfect for stylized assets or experimental image-based mesh generation.

> **Note:** This plugin is currently only available for local use and not yet published on the Godot Asset Library.

---

## Features

- Supports 3 generation modes: `Random`, `Edge`, and `Segment`
- Adjustable color modes: `Single` (flat color) or `Blend` (gradient)
- Built-in mesh generation using Godot’s 2D rendering
- Highly configurable dot spacing, thresholds, and resolution scaling
- Preview and regenerate meshes live in the editor

---

## Installation

1. Copy the plugin folder to your project:
   ```
   res://addons/VectorizerImagePlugin/
   ```

---

## Usage

1. Add a `VectorizeImage` node to your scene.
2. Assign a texture to the **Texture Image** field.
3. Choose a **Generation Mode**:
   - `Random`: Places dots randomly
   - `Edge`: Places dots along detected edges
   - `Segment`: Places dots along color segment boundaries
4. Choose a **Color** mode:
   - `Single`: Uses center color of triangle
   - `Blend`: Averages colors between vertices
5. Adjust relevant parameters:
   - `Down Scale Multiplier`: Reduce input resolution
   - `Edge Threshold`, `Dot Spacing`, `Edge Contrast Threshold`, etc.
6. Enable the **Generate** checkbox to create the mesh.
7. Optionally use the **Preview** field to see your texture overlaid.

## Feedback

Feel free to submit suggestions, issues, or feature requests via [GitHub Issues](https://github.com/your-repo/issues).

