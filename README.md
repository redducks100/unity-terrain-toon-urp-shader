This is an update version of the shader and its hlsl files of: https://github.com/billyBobCletus/UnityURPToonTerrainShader
It should work for Unity 6000.0.24f1.
Feel free to modify and use it as you wish.

Drag and drop these files to your project and create a new material with it and assign it to the terrain.
Make sure your ramp texture import settings are:

- Filter mode: Point (no filter)
- Max Size: 128
- Resize Algorithm: Bilinear
- Compression: None

How to update for future versions:
- Find the shaders for your version of unity here (https://github.com/Unity-Technologies/Graphics) by going through the tags
- Diff check the files and add the changes to the new version: 
  ToonTerrain.shader: (cloned from Packages/com.unity.render-pipelines.universal/Shaders/Terrain/TerrainLit.shader)
  ToonTerrainAdd.shader: (cloned from Packages/com.unity.render-pipelines.universal/Shaders/Terrain/TerrainLitAdd.shader)
  ToonTerrainInput.hlsl: (cloned from Packages/com.unity.render-pipelines.universal/Shaders/Terrain/TerrainLitInput.hlsl)
  ToonTerrainPasses.hlsl: (cloned from Packages/com.unity.render-pipelines.universal/Shaders/Terrain/TerrainLitPasses.hlsl)
