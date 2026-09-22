# Prompt guide

## Agent instruction (paste this)

> You have a folder of 56 reference photos of Dan in `images/`.
> Before each image generation: look at the photos, pick 3 to 6 that best match
> the target shot (same head angle, same light, same mood), and send them as
> reference images with the prompt below. Always say "the man in the reference
> photos" in the prompt. Never describe the face from memory.

## Base identity line

Use this in every prompt:

> The man in the reference photos: mixed-race, short black curly hair with
> faded sides, light stubble, black ear plugs, calm confident face.

## Prompt template

```
[Base identity line], [what he is doing], [where], [lighting], [camera / style].
Keep the face exactly like the reference photos.
```

## Examples

```
The man in the reference photos, sitting at a desk with a laptop, small home studio,
soft window light from the left, 50mm photo, natural colour.
Keep the face exactly like the reference photos.
```

```
The man in the reference photos, on stage holding a microphone, dark venue,
warm spotlight, editorial photo.
Keep the face exactly like the reference photos.
```

## Fixes

- Face looks wrong: use fewer reference photos, closer to the target angle.
- Face too smooth or fake: add "unretouched skin, real photo".
- Still wrong after 5 tries: train a LoRA (see README, training mode).
