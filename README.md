# ActualRobloxFFlags
roblox fastflag list but actually good flags
### quality of life/performance
###### max is 21, Basically override ur quality to 1 and set ur in-game graphics to 10 if u wanna spoof having max graphics for some reason.
``` json
{
    "DFIntDebugFRMQualityLevelOverride": "1"
}
```
###### Improved replication (default 15) this WILL increase outgoing network traffic
``` json
{
    "DFIntS2PhysicsSenderRate": "60"
}
```
###### Faster game launch (Likely to cause bugs)
``` json
{
    "FFlagEnableQuickGameLaunch": "True"
}
```
###### values over 4 cause viewport issues (MSAA is a form of anti-aliasing)
``` json
{
    "FIntDebugForceMSAASamples": "4"
}
```
###### Improves fps by quite a bit (5-100%) but ONLY on windows and it causes issues especially with the game selector screen so launch from the web
``` json
{
    "FFlagMovePrerender": "True",
    "FFlagMovePrerenderV2": "True"
}
```
### renderer types
##### Vulkan | peak performance for Linux only good for newish GPU's works on windows but directX is better for windows
``` json
{
    "FFlagDebugGraphicsDisableDirect3D11": "True",
    "FFlagDebugGraphicsPreferVulkan": "True"
}
```
##### DirectX11 | Newest DirectX available on roblox best for gpu's that are made after like 2010 and good for windows
``` json
{
    "FFlagDebugGraphicsPreferD3D11": "True"
}
```
##### DirectX10 | For windows if u have an old gpu that works better with this one
``` json
{
    "FFlagDebugGraphicsPreferD3D11FL10": "True"
}
```
##### OpenGL | Compatability for old gpu's works on all platforms but lower performance on new gpu's
``` json
{
    "FFlagDebugGraphicsDisableDirect3D11": "True",
    "FFlagDebugGraphicsPreferOpenGL": "True"
}
```
##### Metal | MacOS only rendering system havent tested it since i dont like apple
``` json
{
    "FFlagDebugGraphicsPreferMetal": "True"
}
```
