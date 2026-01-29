# Roblox-Client-Settings

Optimized Roblox client settings for maximum performance. This is a comprehensive collection of flags and configurations that significantly improve performance and visual experience.

## 📋 Table of Contents

- [Performance Optimization (FPS)](#performance-optimization-fps)
- [Graphics Settings](#graphics-settings)
- [Lighting and Shadows](#lighting-and-shadows)
- [Textures and Materials](#textures-and-materials)
- [Visual Effects](#visual-effects)
- [Audio and Chat](#audio-and-chat)
- [Telemetry](#telemetry)
- [Other Optimizations](#other-optimizations)

---

## 🎮 Performance Optimization (FPS)

| Flag | Value | Description |
|------|-------|-------------|
| `DFIntTaskSchedulerTargetFps` | 9999 | Sets target FPS to maximum, allowing your system to run unlimited |
| `FFlagEnableFrameRateManager` | True | Enables frame rate manager |
| `FFlagHandleAltEnterFullscreenManually` | True | Handles fullscreen manually with Alt+Enter |
| `FFlagEnableQuickGameLaunch` | True | Enables quick game launch |
| `DFIntRenderClipPlaneNear` | 5 | Minimum render distance (in studs) |
| `DFIntRenderClipPlaneFar` | 500 | Maximum render distance (in studs) |

---

## 🎨 Graphics Settings

| Flag | Value | Description |
|------|-------|-------------|
| `FFlagFixGraphicsQuality` | True | Fixes graphics quality issues |
| `FFlagDisablePostFx` | True | Disables post-processing effects (bloom, etc.) |
| `DFIntDebugFRMQualityLevelOverride` | 1 | Forces minimum quality level (1=very low) |
| `DFIntGraphicsQualityLevel` | 1 | Set global graphics quality level |
| `FFlagDisableQualityLevelSelection` | True | Disables manual quality selection |
| `FFlagRenderLowDetailCharacters` | True | Reduces character/avatar details |
| `FFlagRenderLowDetailEnvironment` | True | Reduces environment details |
| `FFlagRenderLowDetailModels` | True | Reduces 3D model details |
| `FFlagRenderLowDetailTerrain` | True | Reduces terrain details |

---

## 💡 Lighting and Shadows

| Flag | Value | Description |
|------|-------|-------------|
| `FFlagDisableShadows` | True | Completely disables real-time shadows |
| `FFlagDisableDynamicLights` | True | Disables dynamic lights |
| `FFlagDisableEnvironmentLighting` | True | Disables ambient lighting |
| `FFlagDisablePointLights` | True | Disables point lights |
| `FFlagDisableSpotLights` | True | Disables spot lights |
| `FFlagDisableSurfaceLights` | True | Disables surface lights |
| `FFlagDisableVoxelLighting` | True | Disables voxel lighting |
| `FFlagRenderForceNoShadows` | True | Forces no shadows (reinforces `FFlagDisableShadows`) |
| `FFlagDebugForceFSMCPULightingOnPC` | True | Forces CPU lighting (better performance) |
| `FIntFSMCPULightingPercentage` | 10 | Percentage of lighting processed by CPU (10%) |
| `FFlagDebugForceCPULightCulling` | True | Uses CPU for light culling |
| `FFlagFastGPULightCulling3` | False | Disables fast GPU light culling |
| `FFlagGpuGeometryManager` | False | Disables GPU geometry manager |
| `DFIntDebugLightUpdateMode` | 2 | Light update mode |
| `DFIntLightingDefaultCellsPerAxis` | 1 | Minimum lighting cells per axis |
| `FIntRenderShadowIntensity` | 0 | Shadow intensity (0=disabled) |
| `DFIntRenderShadowmapSize` | 0 | Shadowmap size |
| `DFIntRenderShadowmapResolution` | 0 | Shadowmap resolution |

---

## 🖼️ Textures and Materials

| Flag | Value | Description |
|------|-------|-------------|
| `FFlagDisableTextureStreaming` | True | Disables dynamic texture loading |
| `FFlagDisableAllTextureStreaming` | True | Completely disables texture streaming |
| `FFlagDisableRenderingTextures` | True | Disables texture rendering |
| `DFIntTextureQuality` | 1 | Texture quality (1=very low) |
| `DFIntMaxTextureSize` | 32 | Maximum texture size in pixels |
| `DFIntMaxTextureChannels` | 1 | Maximum number of texture channels |
| `FFlagRenderForceLowQualityTextures` | True | Forces low-quality textures |
| `FIntDefaultMeshCacheSizeMB` | 32 | Mesh cache in MB |
| `DFIntTextureCompositorDefaultMaxTextureSize` | 32 | Compositor maximum texture size |
| `FFlagForceBasicMaterials` | True | Uses only basic materials |
| `FStringPartTexturePackTable2022` | { } | Empty texture package table |
| `DFIntMeshContentProviderForceCacheSize` | 16 | Forced mesh content cache size |
| `FFlagDisableTerrainTextures` | True | Disables terrain textures |
| `FFlagDisableCharacterTextures` | False | Keeps character textures |
| `FFlagDisableEnvironmentTextures` | True | Disables environment textures |
| `FFlagDisableModelTextures` | True | Disables model textures |
| `FFlagDisableUITextures` | False | Keeps UI textures |

---

## ✨ Visual Effects

| Flag | Value | Description |
|------|-------|-------------|
| `FFlagDisableSpecialEffects` | True | Disables special effects |
| `FFlagDisableParticleEffects` | True | Disables particle effects |
| `FFlagDisableStudioSpecialEffects` | True | Disables studio special effects |
| `DFIntParticleMaxCount` | 10 | Maximum particle count (10) |
| `DFIntParticleMaxEmitters` | 5 | Maximum particle emitters (5) |
| `FFlagForceNoDecals` | True | Disables decals completely |
| `FFlagDisableGraphicsDisableDirect3D11` | False | Does not force Direct3D11 disabled |
| `FFlagDebugGraphicsPreferOpenGL` | False | Does not prefer OpenGL |
| `FFlagGraphicsEnableSignal` | False | Disables graphics signals |
| `FIntSSAOBlurPasses` | 0 | SSAO blur passes (0=disabled) |

---

## 🌍 Geometry and Culling

| Flag | Value | Description |
|------|-------|-------------|
| `DFIntCSGLevelOfDetailSwitchingDistance` | 0 | Disables LOD switching for CSG |
| `DFIntCSGLevelOfDetailSwitchingDistanceL12` | 0 | L1-L2 LOD change distance |
| `DFIntCSGLevelOfDetailSwitchingDistanceL23` | 0 | L2-L3 LOD change distance |
| `DFIntCSGLevelOfDetailSwitchingDistanceL34` | 0 | L3-L4 LOD change distance |
| `DFIntCSRMaxStreamedRegionsPerFrame` | 1 | Maximum streaming regions per frame |
| `FFlagStreamingEnabled` | False | Completely disables streaming |
| `FIntStreamingTargetTextureSizeMB` | 16 | Streaming target texture size |
| `FIntTerrainArraySliceSize` | 1 | Terrain array slice size |
| `DFFlagDebugPauseVoxelizer` | True | Pauses voxelizer |
| `DFFlagDebugRenderForceTechnologyVoxel` | False | Does not force voxel technology |
| `FIntFRMMaxGrassDistance` | 0 | Maximum grass distance (0=disabled) |
| `FIntFRMMinGrassDistance` | 0 | Minimum grass distance |
| `FIntFRMMinDistance` | 0 | Minimum far render distance |

---

## 🔇 Audio and Chat

| Flag | Value | Description |
|------|-------|-------------|
| `FFlagEnableAudioOutputDevice` | False | Disables audio device selector |
| `FFlagAudioDeviceSelectorEnabled` | False | Disables audio device selector |
| `FFlagVoiceChatServiceEnabled` | False | Disables voice chat service |
| `DFFlagAvatarChatServiceEnabled` | False | Disables avatar chat service |
| `DFFlagAvatarChatEnableVoiceChat` | False | Disables voice chat on avatars |
| `FFlagSimplifiedChatFilterEnable` | True | Enables simplified chat filter |

---

## 📊 Telemetry

| Flag | Value | Description |
|------|-------|-------------|
| `FFlagDebugDisableTelemetryEphemeralCounter` | True | Disables ephemeral telemetry counter |
| `FFlagDebugDisableTelemetryEphemeralStat` | True | Disables ephemeral telemetry stat |
| `FFlagDebugDisableTelemetryEventIngest` | True | Disables telemetry event ingestion |
| `FFlagDebugDisableTelemetryPoint` | True | Disables telemetry points |
| `FFlagDebugDisableTelemetryV2Counter` | True | Disables V2 telemetry counter |
| `FFlagDebugDisableTelemetryV2Event` | True | Disables V2 telemetry event |
| `FFlagDebugDisableTelemetryV2Stat` | True | Disables V2 telemetry stat |
| `FFlagAdServiceEnabled` | False | Disables ad service |
| `FLogNetwork` | 0 | Network log level (0=disabled) |

---

## 🔧 Other Optimizations

| Flag | Value | Description |
|------|-------|-------------|
| `FFlagPreloadAllFonts` | False | Does not preload all fonts |
| `FFlagPreloadTextures` | False | Does not preload textures |
| `FFlagUseShadowMap` | False | Does not use shadow map |
| `FIntUITextureMaxRenderTextureSize` | 64 | Maximum UI render texture size |
| `FFlagRenderGpuTextureCompressor` | False | Does not use GPU texture compressor |
| `DFIntGPUTextureCompressorWorkerCount` | 1 | GPU texture compressor workers (1) |
| `FIntEmotesAnimationsMemoryCacheSize` | 0 | Emote animations memory cache size |
| `FIntEnableCameraByDefault` | False | Does not enable camera by default |
| `DFIntMaxFrameBufferSize` | 256 | Maximum frame buffer size |
| `FFlagEnableInGameMenuV3` | False | Disables in-game menu V3 |
| `FFlagFacialAnimationStreamingServiceEnabled` | False | Disables facial animation streaming service |
| `FFlagDebugForceMoveToCPU` | True | Moves calculations to CPU |
| `FFlagDisableGPUAcceleration` | False | Does not fully disable GPU acceleration |
| `FFlagDisableHWAcceleration` | False | Does not disable hardware acceleration |
| `FFlagFastLightUpdates` | True | Enables fast light updates |

---

## 💡 How to Use

1. Copy the flags you need for your configuration
2. Navigate to: `%localappdata%\Roblox\Versions\<version>\ClientSettings\`
3. Open or create the `ClientAppSettings.json` file
4. Paste the flags in JSON format
5. Restart Roblox

Or simply use the `roblox-flags.json` file provided in this repository.

**Note:** This configuration prioritizes performance over visual quality. Adjust according to your needs.
