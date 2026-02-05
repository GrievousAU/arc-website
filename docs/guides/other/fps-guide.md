# FPS Guide

> <Badge type="warning" text="Under Review"/>

This FPS guide is intended to help you understand and optimize your Assetto Corsa and Custom Shaders Patch settings.

Optimizing settings is all about balancing quality to performance and depends on what you as the user wants.

:::tip What this guide *CAN* and *CANNOT* do
> This guide will help you understand and optimise your settings for the best balance between quality and performance. Increase and decrease the settings as needed.
>
> This guide WILL NOT magically increase your FPS to 300 at 4k resolution and it will not make your PC itself better if the specs are terrible.
:::
##

::::warning **What are some common causes of FPS issues?**
:::details **`Installing Pure by dragging it into CM.`**
> This causes heavy FPS drops. Follow the video here to install it correctly: https://www.youtube.com/watch?v=KJE2xac5f8s
:::

:::details **`Your CPU/GPU is not strong enough for your monitor resolution.`**
> If you have low-end hardware, avoid resolutions above 1080p. If you use a higher resolution monitor, lower the resolution in your GPU control panel.
:::

:::details **`Shadow and/or reflection resolution are set too high.`**
> Values between 3K–8K are usually overkill. For low- to mid-tier PCs, keep this at 1024–2048.
:::

:::details **`MSAA is set to 8x.`**
> Use 2x/turn it off on low-end systems, and 4x max if your PC can handle it.
:::

:::details **`Rain.`**
> Avoid using this if you’re in need of more frames.
:::

:::details **`Tree skins.`**
> While they can drastically change the look of maps, its not recommended to use them if you are using low to mid-tier hardware.
:::
::::

##

::::info **Assetto Corsa Video Settings**

:::details **Resolution and FPS:**
### `Rendering Mode:`
> Set to match your screen set up i.e One Monitor = Single Screen.
> Tick fullscreen as windowed mode usually diminishes frames.

### `Resolution:`
> Set this to match your monitor's resolution and refresh rate.
> Please note that the higher your resolution, the more demanding it is on your FPS.

> Do not enable `Fix Resolution Automatically`, `Vertical Synchronization`, or `Limit framerate`.
:::

:::details **Quality:**
### `MSAA:`
> Set to `2x` or `4x` depending on PC specs <br>
> Do not use `8x`.

### `Anisotropic Filtering:`
> Feel free to max this out.

### `World Details:`
> This is reliant on the track you are using but usually set this to `Medium` or `High`.

### `Shadow Resolution:`
> This is the biggest frame killer, set this to `512x512` or `1024x1024` <br>
> **NEVER** set this to anything above `2048x2048`.

### `Smoke Generation:`
> This setting is overridden by ParticlesFX but you can set this to `Medium` anyways.
:::

:::details **Reflections:**
### `Reflection Resolution:`
> Set this to either `512x512` or `1024x1024`.

### `Reflection Frequency:`
> **ONLY** set this to `Two face per frame`.

### `Rendering Distance:`
> Feel free to max this out.
:::

:::details **Post-Processing:**
### `Enable Post-Processing Effects`
> Have this checked/enabled.

### `Filter:`
> Depending on the filter you use, the impact can vary but usually the `defaults` and the `pure_` (if pure is installed) ones are the best for FPS.

### `Overall Quality:`
> Setting this to `High` or `Very High` should be sufficient.

### `Glare Quality:`
> Setting this to `High` or `Very High` should be sufficient.

### `Depth of Field:`
> Setting this to `Maximum` is fine as it only works during replays.

### `Motion Blur:`
> Set this to `Off`

### `Saturation:`
> Leave this at 100%

### `Heat Shimmering`
> You can leave this off as it is not noticeable and can take some frames

### `Sunrays`
> Leave this on

### `FXAA`
> Leave this on
:::

:::details **Mirrors:**
### `Mirror Resolution:`
> `128x512` or `256x1024` is sufficient and should provide a good balance.

### `High Quality`
> Leave this on
:::
::::

##

:::::info Custom Shaders Patch Settings
::::details Version 0.3.X

:::details `CSP Settings > Other > DXGI`
> - Make sure you have “Pace frames better” & set Maximum latency to 1 frame.
:::

:::details `CSP settings > Patch > Optimizations`
> - Under CPU optimizations, make sure you have “Flatten nodes” & "Apply hyperthreading fix" checked <br>
> - Set Chunks optimization to “Advanced”. <br>
> - Under GPU optimizations enable "Optimize meshes" <br>
>
> Some maps may be incompatible with Chunks Optimization so if you have issues with textures, try disabling it first.
:::
<br>

**If you followed the first 2 steps & still have low fps apply these changes aswell:**
<br>

:::details `Custom Shaders Patch Settings:`
> - `Graphics > LightningFX > Dynamic Shadows off` <br>
> <br>
> - `Graphics > ParticleFX > Sparks off` <br>
> - `Graphics > ParticleFX > Fireworks off` <br>
> - `Graphics > ParticleFX > Solid Pieces off` <br>
> <br>
> - `Cars > Windscreen FX > Remove dirt completely on` <br>
> <br>
> - `Cars > Visual > Tyres FX > off` <br>
> - `Cars > Visual > Brake Discs > off` <br>
> <br>
> - `Track > GrassFX > off` <br>
> <br>
> - `Track > SkidmarksFX> set limit to 20k or lower` <br>
:::

:::details `Assetto Corsa Video Settings:`
> - Enable Triple Buffering 
> - Lower MSAA
> - Lower Shadow Resolution
> - Lower Smoke Generation
> - Lower Reflection Resolution
> - Lower Mirror Resolution
:::
<br>

**If you still need fps and the above changes did not work, use this as a last resort.** <br>
**Be warned that they have the largest impact on your graphics.**
<br>

:::details `Custom Shaders Patch Settings:`
> - **Only use these last two options when you desperately need the FPS, out of the entire guide they affect your graphics the most.**
> - Graphics > ExtraFX > Uncheck active
> - Graphics > Adjustments > AMD FidelityFX Super Resolution (FSR) <br>
> (Lower % presets look worse, but give bigger FPS boosts.)
:::
::::

::::details Version 0.2.X
:::details `CSP Settings > DXGI`
> - Make sure you have “Use new dxgi flip model” & “Triple buffering” checked
> - Set Maximum latency to 1 frame.
:::

:::details `CSP settings > General Patch Settings > GPU & CPU optimizations`
> - Under CPU optimizations, make sure you have “Flatten nodes” & "Apply hyperthreading fix" checked <br>
> - Set Chunks optimization to “Advanced (experimental)”. <br>
> - Under GPU optimizations, enable "Optimize meshes" & "Optimize messhes some more" <br>
>
> Some maps may be incompatible with Chunks Optimization so if you have issues with textures, try disabling it first.
:::
<br>

**If you followed the first 2 steps & still have low fps apply these changes aswell:**
<br>

:::details `Custom Shaders Patch Settings:`
> - `LightningFX > Dynamic Shadows off` <br>
> <br>
> - `GrassFX > off` <br>
> <br>
> - `ParticleFX > Sparks off` <br>
> - `ParticleFX > Fireworks off` <br>
> - `ParticleFX > Solid Pieces off` <br>
> <br>
> - `WindscreenFX > Remove dirt completely on` <br>
> <br>
> - `Brake DiscFX > off` <br>
> <br>
> - `SkidmarksFX> set limit to 20k or lower` <br>
:::

:::details `Assetto Corsa Video Settings:`
> - Enable Triple Buffering 
> - Lower MSAA
> - Lower Shadow Resolution
> - Lower Smoke Generation
> - Lower Reflection Resolution
> - Lower Mirror Resolution
:::
<br>

**If you still need fps and the above changes did not work, use this as a last resort.** <br>
**Be warned that they have the largest impact on your graphics.**
<br>

:::details `Custom Shaders Patch Settings:`
> - **Only use these last two options when you desperately need the FPS, out of the entire guide they affect your graphics the most.**
> - Graphics > ExtraFX > Uncheck active
> - Graphics > Adjustments > AMD FidelityFX Super Resolution (FSR) <br>
> (Lower % presets look worse, but give bigger FPS boosts.)
:::
::::
:::::
