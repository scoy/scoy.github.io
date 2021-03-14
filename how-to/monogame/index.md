---
title: InfiniteInstant
subtitle: Dev Notes
layout: page
hero_height: is-small
show_sidebar: false
---

# MonoGame

Getting content to show up in VS while also being in MGCB.

To add content to a VS project:
- Find the folder with Content.mgcb in it.  This should be named 'Content'.
- Copy/Paste folders or files into here.  
- For folders, you then need to drag them into the Solution Explorer.  This will give the a name appended by -Copy.  Delete the originals in Windows Explorer and then rename them in Solution Explorer.
- For files, use the Add Existing Item option.  The files should have **Build Action: Content** and **Copy to Output Directory: Do not copy** already set. 
- In MGCB Editor, use the Add Existing option to add folders or files.  Note that adding a folder with other, nested folders will clone the nested folders to the same level.  Remove these from both MGCB and via Windows Explorer.

This should make it easy to see the current content and to edit shaders.  Note that this must be kept in sync manually.