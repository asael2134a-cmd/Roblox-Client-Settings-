# Roblox-Client-Settings-

Configuración optimizada del cliente Roblox para rendimiento máximo. Esta es una colección exhaustiva de flags y configuraciones que mejoran significativamente el rendimiento y la experiencia visual.

## 📋 Tabla de Contenidos

- [Optimización de Rendimiento (FPS)](#optimización-de-rendimiento-fps)
- [Configuración de Gráficos](#configuración-de-gráficos)
- [Iluminación y Sombras](#iluminación-y-sombras)
- [Texturas y Materiales](#texturas-y-materiales)
- [Efectos Visuales](#efectos-visuales)
- [Audio y Chat](#audio-y-chat)
- [Telemetría](#telemetría)
- [Otras Optimizaciones](#otras-optimizaciones)

---

## 🎮 Optimización de Rendimiento (FPS)

| Flag | Valor | Descripción |
|------|-------|-------------|
| `DFIntTaskSchedulerTargetFps` | 9999 | Establece el FPS objetivo a máximo, permitiendo que tu sistema rinda sin límites |
| `FFlagEnableFrameRateManager` | True | Activa el gestor de velocidad de fotogramas |
| `FFlagHandleAltEnterFullscreenManually` | True | Maneja la pantalla completa manualmente con Alt+Enter |
| `FFlagEnableQuickGameLaunch` | True | Permite iniciar juegos más rápidamente |
| `DFIntRenderClipPlaneNear` | 5 | Distancia mínima de renderizado (en studs) |
| `DFIntRenderClipPlaneFar` | 500 | Distancia máxima de renderizado (en studs) |

---

## 🎨 Configuración de Gráficos

| Flag | Valor | Descripción |
|------|-------|-------------|
| `FFlagFixGraphicsQuality` | True | Corrige problemas de calidad gráfica |
| `FFlagDisablePostFx` | True | Desactiva efectos post-procesamiento (bloom, etc.) |
| `DFIntDebugFRMQualityLevelOverride` | 1 | Fuerza nivel de calidad mínimo (1=muy bajo) |
| `DFIntGraphicsQualityLevel` | 1 | Establecer nivel de calidad gráfica global |
| `FFlagDisableQualityLevelSelection` | True | Desactiva la selección manual de calidad |
| `FFlagRenderLowDetailCharacters` | True | Reduce detalles en caracteres/avatares |
| `FFlagRenderLowDetailEnvironment` | True | Reduce detalles en el entorno |
| `FFlagRenderLowDetailModels` | True | Reduce detalles en modelos 3D |
| `FFlagRenderLowDetailTerrain` | True | Reduce detalles en el terreno |

---

## 💡 Iluminación y Sombras

| Flag | Valor | Descripción |
|------|-------|-------------|
| `FFlagDisableShadows` | True | Desactiva completamente las sombras en tiempo real |
| `FFlagDisableDynamicLights` | True | Desactiva luces dinámicas |
| `FFlagDisableEnvironmentLighting` | True | Desactiva iluminación ambiental |
| `FFlagDisablePointLights` | True | Desactiva luces puntuales |
| `FFlagDisableSpotLights` | True | Desactiva focos de luz |
| `FFlagDisableSurfaceLights` | True | Desactiva luces de superficie |
| `FFlagDisableVoxelLighting` | True | Desactiva iluminación voxel |
| `FFlagRenderForceNoShadows` | True | Fuerza sin sombras (refuerza `FFlagDisableShadows`) |
| `FFlagDebugForceFSMCPULightingOnPC` | True | Fuerza iluminación por CPU (mejor rendimiento) |
| `FIntFSMCPULightingPercentage` | 10 | Porcentaje de iluminación procesada por CPU (10%) |
| `FFlagDebugForceCPULightCulling` | True | Usa CPU para culling de luces |
| `FFlagFastGPULightCulling3` | False | Desactiva fast GPU light culling |
| `FFlagGpuGeometryManager` | False | Desactiva gestor de geometría GPU |
| `DFIntDebugLightUpdateMode` | 2 | Modo de actualización de luces |
| `DFIntLightingDefaultCellsPerAxis` | 1 | Celdas mínimas de iluminación por eje |
| `FIntRenderShadowIntensity` | 0 | Intensidad de sombras (0=desactivado) |
| `DFIntRenderShadowmapSize` | 0 | Tamaño del mapa de sombras |
| `DFIntRenderShadowmapResolution` | 0 | Resolución del mapa de sombras |

---

## 🖼️ Texturas y Materiales

| Flag | Valor | Descripción |
|------|-------|-------------|
| `FFlagDisableTextureStreaming` | True | Desactiva carga dinámica de texturas |
| `FFlagDisableAllTextureStreaming` | True | Desactiva completamente streaming de texturas |
| `FFlagDisableRenderingTextures` | True | Desactiva renderizado de texturas |
| `DFIntTextureQuality` | 1 | Calidad de texturas (1=muy baja) |
| `DFIntMaxTextureSize` | 32 | Tamaño máximo de textura en píxeles |
| `DFIntMaxTextureChannels` | 1 | Número máximo de canales de textura |
| `FFlagRenderForceLowQualityTextures` | True | Fuerza texturas de baja calidad |
| `FIntDefaultMeshCacheSizeMB` | 32 | Caché de malla en MB |
| `DFIntTextureCompositorDefaultMaxTextureSize` | 32 | Tamaño máximo de textura del compositor |
| `FFlagForceBasicMaterials` | True | Usa solo materiales básicos |
| `FStringPartTexturePackTable2022` | { } | Tabla de paquetes de texturas vacía |
| `DFIntMeshContentProviderForceCacheSize` | 16 | Tamaño forzado de caché de contenido de malla |
| `FFlagDisableTerrainTextures` | True | Desactiva texturas de terreno |
| `FFlagDisableCharacterTextures` | False | Mantiene texturas de personaje |
| `FFlagDisableEnvironmentTextures` | True | Desactiva texturas del entorno |
| `FFlagDisableModelTextures` | True | Desactiva texturas de modelos |
| `FFlagDisableUITextures` | False | Mantiene texturas de UI |

---

## ✨ Efectos Visuales

| Flag | Valor | Descripción |
|------|-------|-------------|
| `FFlagDisableSpecialEffects` | True | Desactiva efectos especiales |
| `FFlagDisableParticleEffects` | True | Desactiva efectos de partículas |
| `FFlagDisableStudioSpecialEffects` | True | Desactiva efectos especiales en Studio |
| `DFIntParticleMaxCount` | 10 | Número máximo de partículas (10) |
| `DFIntParticleMaxEmitters` | 5 | Número máximo de emisores de partículas (5) |
| `FFlagForceNoDecals` | True | Desactiva decals completamente |
| `FFlagDisableGraphicsDisableDirect3D11` | False | No fuerza desactivar Direct3D11 |
| `FFlagDebugGraphicsPreferOpenGL` | False | No prefiere OpenGL |
| `FFlagGraphicsEnableSignal` | False | Desactiva señales gráficas |
| `FIntSSAOBlurPasses` | 0 | Pases de desenfoque SSAO (0=desactivado) |

---

## 🌍 Geometría y Culling

| Flag | Valor | Descripción |
|------|-------|-------------|
| `DFIntCSGLevelOfDetailSwitchingDistance` | 0 | Desactiva LOD switching para CSG |
| `DFIntCSGLevelOfDetailSwitchingDistanceL12` | 0 | Distancia de cambio LOD L1-L2 |
| `DFIntCSGLevelOfDetailSwitchingDistanceL23` | 0 | Distancia de cambio LOD L2-L3 |
| `DFIntCSGLevelOfDetailSwitchingDistanceL34` | 0 | Distancia de cambio LOD L3-L4 |
| `DFIntCSRMaxStreamedRegionsPerFrame` | 1 | Regiones máximas de streaming por fotograma |
| `FFlagStreamingEnabled` | False | Desactiva streaming completamente |
| `FIntStreamingTargetTextureSizeMB` | 16 | Tamaño objetivo de textura de streaming |
| `FIntTerrainArraySliceSize` | 1 | Tamaño de slice de array de terreno |
| `DFFlagDebugPauseVoxelizer` | True | Pausa el voxelizador |
| `DFFlagDebugRenderForceTechnologyVoxel` | False | No fuerza tecnología voxel |
| `FIntFRMMaxGrassDistance` | 0 | Distancia máxima de pasto (0=desactivado) |
| `FIntFRMMinGrassDistance` | 0 | Distancia mínima de pasto |
| `FIntFRMMinDistance` | 0 | Distancia mínima de renderizado lejano |

---

## 🔇 Audio y Chat

| Flag | Valor | Descripción |
|------|-------|-------------|
| `FFlagEnableAudioOutputDevice` | False | Desactiva selector de dispositivo de audio |
| `FFlagAudioDeviceSelectorEnabled` | False | Desactiva selector de dispositivo de audio |
| `FFlagVoiceChatServiceEnabled` | False | Desactiva servicio de chat de voz |
| `DFFlagAvatarChatServiceEnabled` | False | Desactiva servicio de chat de avatar |
| `DFFlagAvatarChatEnableVoiceChat` | False | Desactiva chat de voz en avatares |
| `FFlagSimplifiedChatFilterEnable` | True | Activa filtro de chat simplificado |

---

## 📊 Telemetría

| Flag | Valor | Descripción |
|------|-------|-------------|
| `FFlagDebugDisableTelemetryEphemeralCounter` | True | Desactiva contador telemetría efímera |
| `FFlagDebugDisableTelemetryEphemeralStat` | True | Desactiva estadística telemetría efímera |
| `FFlagDebugDisableTelemetryEventIngest` | True | Desactiva ingesta de eventos telemetría |
| `FFlagDebugDisableTelemetryPoint` | True | Desactiva puntos de telemetría |
| `FFlagDebugDisableTelemetryV2Counter` | True | Desactiva contador V2 de telemetría |
| `FFlagDebugDisableTelemetryV2Event` | True | Desactiva evento V2 de telemetría |
| `FFlagDebugDisableTelemetryV2Stat` | True | Desactiva estadística V2 de telemetría |
| `FFlagAdServiceEnabled` | False | Desactiva servicio de anuncios |
| `FLogNetwork` | 0 | Nivel de log de red (0=desactivado) |

---

## 🔧 Otras Optimizaciones

| Flag | Valor | Descripción |
|------|-------|-------------|
| `FFlagPreloadAllFonts` | False | No precarga todas las fuentes |
| `FFlagPreloadTextures` | False | No precarga texturas |
| `FFlagUseShadowMap` | False | No usa mapa de sombras |
| `FIntUITextureMaxRenderTextureSize` | 64 | Tamaño máximo de textura UI renderizada |
| `FFlagRenderGpuTextureCompressor` | False | No usa compresor GPU de texturas |
| `DFIntGPUTextureCompressorWorkerCount` | 1 | Trabajadores compresor GPU (1) |
| `FIntEmotesAnimationsMemoryCacheSize` | 0 | Caché de memoria para animaciones de emotes |
| `FIntEnableCameraByDefault` | False | No habilita cámara por defecto |
| `DFIntMaxFrameBufferSize` | 256 | Tamaño máximo del buffer de fotogramas |
| `FFlagEnableInGameMenuV3` | False | Desactiva menú en juego V3 |
| `FFlagFacialAnimationStreamingServiceEnabled` | False | Desactiva servicio de streaming de animación facial |
| `FFlagDebugForceMoveToCPU` | True | Mueve cálculos a CPU |
| `FFlagDisableGPUAcceleration` | False | No desactiva aceleración GPU completamente |
| `FFlagDisableHWAcceleration` | False | No desactiva aceleración hardware |
| `FFlagFastLightUpdates` | True | Habilita actualizaciones rápidas de luces |

---

## 💡 Cómo Usar

1. Copia los flags que necesites según tu configuración
2. Navega a: `%localappdata%\Roblox\Versions\<version>\ClientSettings\`
3. Abre o crea archivo `ClientAppSettings.json`
4. Pega los flags en formato JSON
5. Reinicia Roblox

**Nota:** Esta configuración prioriza el rendimiento sobre la calidad visual. Ajusta según tus necesidades.
