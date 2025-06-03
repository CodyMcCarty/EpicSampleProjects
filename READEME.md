# Epic Sample Projects

### This is a collection of Unreal Assets from Epic's many sample projects
todos important: 
- [ ] insert pic, from awesome demo map
- [x] lisense
- [ ] avoid LFS
- [ ] clean up my github?
- [ ] notes about Kenshi, Warband, Guild 2 Renaissance.

# Introduction
Epic Games has released many high-quality sample projects over the years, each containing useful assets like characters, trees, shields, vehicles, props, and more. However, these assets are spread across dozens of large projects, making it inefficient and time-consuming to find and reuse them.

This project solves that problem by centralizing a curated collection of assets from Epic's sample projects into a single location. Instead of loading and searching through multiple multi-gigabyte projects just to find one asset, developers can browse this consolidated repository.  Additionally, many of the assets have be cleaned up.

Key goals:

- Convenience: Avoid having to open and search individual sample projects to extract a single asset.
- Curation: Includes ~70–80% of the most generally useful assets (excluding ones with limited utility).
- Preservation: Maintains a branch with original, unmodified versions of assets for reference and backup in UE v4.26.
- Organization: Assets are renamed and reorganized into categorized folders for easier discovery and reuse.
- Future Utility: Intended to eventually support standardized materials and setups for quicker integration into new projects.

This project simplifies asset reuse, reduces storage bloat, and saves developers time — especially when prototyping or working across multiple Unreal projects.

# Key changes from original work
# How to Use
The assets are in a content plugin.  There are issues using assets this way. You will need correct use of `Migrate` vs `Move`

Assets can be `Migrated` from Plugin to Plugin and from Game to Game.   However, they cannot be `Moved`.  
Assets can be `Moved` from Plugin to Game and from Game to Plugin.  
To use assets, first `Migrate` them to another plugin, then if needed, `Move` them from your plugin to your game.  This will avoid asset references breaking when they expect Plugin\Content vs Game\Content (only move handles this correctly).  
I understand this is complicated, and will be fixed latter.
### Pre-reqs
# Roadmap
- [ ] Move from a material layer work flow to a material instance workflow
- [ ] make a few master materials
- [ ] Reorganize and reconsolidate: 
  - [ ] There are many duplicate textures that need to be condensed. 
  - [ ] The folder structure is currently by sample project, I need to make the structure as if it was one project.
- [ ] Move from content plugin to project. There are issues with moving/migrating uassets between plugins and projects. 
- [ ] Skele Meshes need a lot of work to be more useable. 
  - [ ] The characters from the infiltration demo use many materials.
  - [ ] Skele meshes don't share the UE skeleton
  - [ ] They need ABP 
  - [ ] They need to be playable from the get go.
  - [ ] Rendering cost are way to high
- [ ] The assests from SciFiHallway are janky. Clean them up.
- [ ] edit foliage from masked to nanite

# Contributing
IDK yet, hit me up.
# Changes and special notes
There are a few assets I've modified listed here:
- todo

Some projects were skipped, listed here:
- Using Magic Leap in Unreal Engine [course](https://dev.epicgames.com/community/learning/courses/Ml7/using-magic-leap-in-unreal-engine/pbx/introducing-using-magic-leap-in-unreal-engine) and [fab](https://www.fab.com/listings/db323410-5259-45e9-897f-01943ef4317e). I couldn't get the project to load. there are a few office, computer, keyboard assets I would've like to add.
- [Content Examples](https://www.fab.com/listings/4d251261-d98c-48e2-baee-8f4e47c67091): I think it's worth keeping a version of 4.26 and the newest one.
- [Automotive Materials](https://www.fab.com/listings/5dd132fe-ee32-4e8c-9cd3-7496547dfb29) and [docs](https://dev.epicgames.com/documentation/en-us/unreal-engine/automotive-materials-pack-in-unreal-engine?application_version=5.4). It's just too much, but worth checking out. I may get a few detail normals from there.
- [Photorealistic Character](https://www.fab.com/listings/0e9c4282-b266-4778-bab0-f60ac923bb9a) and [docs](https://dev.epicgames.com/documentation/en-us/unreal-engine/photorealistic-character?application_version=4.27). Also known as Digital Human. Again, just too much.

I skipped many animations (not all). Pitchfork Academy (MizzoFrizzo & Co.) already did that work, plus there are many animation available else where.
- 120+ animations, created using a universal humanoid rig, which is compatible with UE: [Quaternius' Universal Animation Library](https://quaternius.com/packs/universalanimationlibrary.html)
-  tonne of free animations taken from the motion matching sample project, the Lyra starter game, and the Advanced Locomotion System V4, as well as the Military Weapons asset packs, you can download them all [right here Pitchfork Academy (MizzoFrizzo & Co.)](https://youtu.be/_-03eby70e0?si=TFu_Gpc67hGCUsIx)
-  And of course [Mixamo](https://www.mixamo.com/#/)'s animations
-  [Animation Starter Pack](https://www.fab.com/listings/98ff449d-79db-4f54-9303-75486c4fb9d9)
