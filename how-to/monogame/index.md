---
title: InfiniteInstant
subtitle: Dev Notes
layout: page
hero_height: is-small
show_sidebar: false
---

# MonoGame

## Setting up a new project from a new VS project.
- Create a new DX project in VS using the project name you want.  By default this should be in **C:\GitHub\MonoGame\Apps\Project**
- Copy .gitignore from EmptyDX (or any other C# project) into the new project's root folder.
- In GitHub Desktop, create the new repository for this and publish to GitHub.
- In Git Bash:
  - cd to /c/GitHub/MonoGame/Apps/Project
  - **$ git submodule init**
  - **$ git submodule add https://github.com/scoy/Koi**
  - cd to /c/GitHub/MonoGame/Apps/Project/Project
  - **$ git submodule add https://github.com/scoy/KoiX**
  - cd to /c/GitHub/MonoGame/Apps/Project/Project/Content
  - **$ git submodule add https://github.com/scoy/KoiXContent**
- Back to VS:
  - Right click on the Solution and add Koi as an existing project.
  - Under Project Dependencies, right click and add project reference to Koi.
  - Under Content, add folders for Audio, Fonts, Textures, Shaders, and Xml as needed.
  - Double-click on the Content.mgcb object to bring up the editor.
  - In the MGCB Editor:
    - Edit->Add Existing Folder and add KoiXContent.  This will replicate the folders inside.  Just right click on them and exclude them.
    - Also need to exclude .git and .gitattribute files from content.
    - Some files need to be set to copy rather than build.
      - Color.fx
      - *.inc
      - All files in Shaders\Filters\Geometry\Code
      - *.txt files in Xml\Unicode
- Should be good to go.  At this point, replace Game1.cs from EmptyDX and add Main.cs.

## Getting content to show up in VS while also being in MGCB.

To add content to a VS project:
- Find the folder with Content.mgcb in it.  This should be named 'Content'.
- Copy/Paste folders or files into here.  
- For folders, you then need to drag them into the Solution Explorer.  This will give the a name appended by -Copy.  Delete the originals in Windows Explorer and then rename them in Solution Explorer.
- For files, use the Add Existing Item option.  The files should have **Build Action: Content** and **Copy to Output Directory: Do not copy** already set. 
- In MGCB Editor, use the Add Existing option to add folders or files.  Note that adding a folder with other, nested folders will clone the nested folders to the same level.  Remove these from both MGCB and via Windows Explorer.

This should make it easy to see the current content and to edit shaders.  Note that this must be kept in sync manually.