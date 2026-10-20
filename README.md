# ViTMatte

The ViTMatte image matting model by Hust Vision Lab, as ONNX and Core ML files.
**ViTMatte is not an ONYX OFX model:** it is published by its authors under their own
license.

## Source and license

- Model: ViTMatte by Hust Vision Lab — https://github.com/hustvl/ViTMatte.
- License: MIT License, Copyright (c) 2023 Hust Vision Lab.
  [LICENSE-ViTMatte](LICENSE-ViTMatte) is the LICENSE file of the ViTMatte repository,
  unchanged: https://github.com/hustvl/ViTMatte/blob/main/LICENSE
- A project maintainer stated publicly that the model weights may be used under the
  MIT terms: https://github.com/hustvl/ViTMatte/issues/9 (the maintainer's statement,
  quoted here for reference, not a statement by ONYX OFX).
- `model.onnx`: the ONNX conversion by "Xenova" —
  https://huggingface.co/Xenova/vitmatte-base-composition-1k (a conversion of
  hustvl/vitmatte-base-composition-1k), hosted here unchanged (revision
  `1290b014b994e95ca1b9dd9c5f72c3b6d5b7236a`). ONYX OFX did not create it.
- `vitmatte-*`: a Core ML conversion of the same model, made by ONYX OFX.

## Your responsibility

ONYX OFX makes no representation as to what the ViTMatte license permits. Please read
the license and make sure your use complies before any commercial use. ONYX OFX hosts
these files as is, without warranty of any kind, and is not affiliated with or endorsed
by their authors.

## Files — release `refiners-v2`

| File | Format | Bytes | SHA-256 |
|---|---|---:|---|
| `model.onnx` | ONNX | 387 371 620 | `f6978437f5068849bcbf49b1f4e37b90aaca5155744e9fde4e6c689f70c2b9ee` |
| `vitmatte-Manifest.json` | Core ML | 617 | `e9a3e03793b99badd027d8050484edef0bac0aa09582f82173d50b112b03420d` |
| `vitmatte-model.mlmodel` | Core ML | 413 330 | `7e56b0b2a18772d97175149ac6e6fd1dbc7e6cec4003294e1262a20839e7b0f3` |
| `vitmatte-weight.bin` | Core ML | 194 862 240 | `1f09ec31119b267bba35aa39ebb9fe77ef60b5a68b7922c26d0c5c9cd9fdd5d2` |
| `LICENSE-ViTMatte` | text | 1 071 | `14d074b534e2301f5d035d6425868d2627530d36e5be81e0a62876f7e8ecd108` |

The three `vitmatte-*` files are the parts of one Core ML package:
`model.mlpackage/Manifest.json`, `model.mlpackage/Data/com.apple.CoreML/model.mlmodel`
and `model.mlpackage/Data/com.apple.CoreML/weights/weight.bin`.

Questions: support@onyxofx.com
