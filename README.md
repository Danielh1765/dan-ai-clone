# Dan AI Clone — reference photos

Private reference set for generating images that look like Dan.

## What is here

- `images/` — 56 photos, JPG, max 2048 px on the long edge.
- `PROMPT_GUIDE.md` — how to use these photos with an image model or agent.

Source: iPhone HEIC photos, converted to JPG so AI tools can read them.
Originals stay on Dan's Mac, not in this repo.

## How to use this

There are two ways to make an AI clone. Both need many photos, not one or two.

**1. Reference mode (fast, no training).**
Give an image model 3 to 6 photos as reference and a prompt.
Works with Nano Banana (Gemini), GPT Image, Flux Kontext, Midjourney (`--cref`).
An agent should read this whole folder, then pick the best photos for the shot
(matching angle, light, expression) and send those. Sending all 56 at once is worse,
not better. Models blur the face when given too many.

**2. Training mode (slow, best likeness).**
Train a LoRA (a small add-on model that learns one face) on all 56 photos.
Use Flux LoRA training on fal.ai or Replicate. Takes 15 to 30 minutes.
After that you type a prompt and get Dan without sending any photos.

Start with 1. Move to 2 if the face is not right.

## Photo set notes

- Front, three-quarter and profile angles.
- Neutral, smiling and laughing expressions.
- Indoor, natural light. Dark T-shirt or fleece.
- Short black curly hair, faded sides, light stubble, ear plugs.

## Rules

- Keep this repo private. These are Dan's face photos.
- Do not add other people's photos here.
