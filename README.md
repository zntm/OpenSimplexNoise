# OpenSimplexNoise

---

A GameMaker extension implementation of [OpenSimplexNoise](https://github.com/deerel/OpenSimplexNoise).

### 🛠️ Features
- #### 🌍 2D / 3D / 4D Noise
    Generate smooth coherent noise for terrain, textures, animation, and procedural effects.

- #### ⚡ Amplitude & Octave
    Includes amplitude and octave parameters to easily control the noise values.

- #### 🎲 Seeding Support
    Initialize the noise generator with any 64-bit seed for reproducible randomness.

### ✏️ Example Usage

```gml
open_simplex_noise_seed(1);

// NOTE: Amplitudes set as 255, and octaves as 8
var _2d = open_simplex_noise(0, 0, 255, 8);
var _3d = open_simplex_noise_3d(0, 0, 255, 8);
var _4d = open_simplex_noise_4d(0, 0, 255, 8);
```

### 📊 Benchmarks

| Size    | 2D Time | 3D Time  | 4D Time    |
| ------- | ------- | -------- | ---------- |
| 16^n    | 0.23 ms | 9.89 ms  | 520.02 ms  |
| 64^n    | 0.80 ms | 65.26 ms | 7830.03 ms |
