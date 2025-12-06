# Vinyl Record Tutorial Examples

These JSON files accompany the tutorial "Dials, Not Dice: A Precision Prompting Guide for Nano Banana Pro."

## Files

| File | Description |
|------|-------------|
| `01-base-render.json` | The initial vinyl record product shot specification |
| `02-lighting-change.json` | Same spec with lighting moved from right to left, intensity reduced |
| `03-camera-angle-change.json` | Same spec with camera angle changed to top-down |

## How to Use

1. Copy the contents of any JSON file
2. Open Nano Banana Pro (Gemini app with "Thinking" model, or Google AI Studio)
3. Paste with the instruction: "Render this specification as a high-fidelity product photograph"
4. Compare renders to see how changing single fields affects the output

## Diffing the Files

To see exactly what changed between versions:

```bash
diff 01-base-render.json 02-lighting-change.json
diff 01-base-render.json 03-camera-angle-change.json
```

The changes are minimal and targeted - that's the whole point of structured prompting.

## Results

The rendered images are in the `images` directory, with refined versions in the `refined_images` subfolder.

### Original Image Prompts

These are the baseline renders using the standard prompt with each JSON specification:

| Image | Prompt | JSON Change | Seed Image(s) |
|-------|--------|-------------|---------------|
| 01-base-render.png | Render this specification as a high-fidelity product photograph. `paste json here` | Base vinyl record specification | None |
| 02-lighting-change.png | Render this specification as a high-fidelity product photograph. `paste json here` | Same spec with lighting moved from right to left, intensity reduced | `01-base-render.png` |
| 03-camera-angle-change.png | Render this specification as a high-fidelity product photograph. `paste json here` | Same spec with camera angle changed to top-down | `01-base-render.png`, `02-lighting-change.png` |

### Refined Image Prompts

These are improved renders using enhanced prompts that provide additional context to the model:

| Image | Prompt | JSON Change | Seed Image(s) |
|-------|--------|-------------|---------------|
| 01-base-render.png | Render this specification as a high-fidelity product photograph. Include the brand_name on the record label | Base vinyl record specification | None |
| 02-lighting-change.png | Render this specification as a high-fidelity product photograph. Include the brand_name on the record label | Same spec with lighting moved from right to left, intensity reduced | `01-base-render.png` |
| 03-camera-angle-change.png | Render this specification as a high-fidelity product photograph. Include the brand_name on the record label, the camera.angle is also important | "camera": { "angle": "overhead",...}" | `01-base-render.png`, `02-lighting-change.png` |



