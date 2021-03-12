---
title: InfiniteInstant
subtitle: How-To
layout: page
show_sidebar: false
---

# Working with SubModules in Git
GitHub Desktop doesn't seem to know much about submodules so it's not a lot of help.  We will use submodules as a way of including libraries into projects without running into the issues we had where all projects shared the same library references.

Most of this is from <https://git-scm.com/book/en/v2/Git-Tools-Submodules>

## Adding a Submodule to a Project
In Git Bash, cd to the folder for the project you want to add the submodule to.  For instance, cd to /c/gitHub/MonoGame/Apps/AppFoo then add the submodule.<br>
**$ git submodule add URL**<br>
where URL is the URL of the submodule e.g. **https://github.com/scoy/Koi**<br>
This will create a new folder in the current location with the name of the included submodule.

**$ ls** will show:<br>
**AppFoo/ AppFoo.sln Koi/**

Now in Visual Studio add the submodule project to the app's solution (Add existing project -- nav to the submodule's .csproj file).  You will also need to add a project reference in the app to the submodule project. 

## Seeing Local Changes
If you've changed the submodel, GitHub Desktop will let you know bu showing a change in the submodule but won't allow you to do anything about it.  Here's what it looks like when both Koi and Koi.Prim2D have been changed.
![GitHub Dekstop](desktop.png)
In Bash you can see the actual changes using sdiff.  sdiff is and alias (submodule diff) that has been defined as<br>
**$ git config alias.sdiff '!'"git diff && git submodule foreach 'git diff'"**
Typing **$ git sdiff** results in:<br>
```
$ git sdiff
diff --git a/Koi b/Koi
--- a/Koi
+++ b/Koi
@@ -1 +1 @@
-Subproject commit 2772822d69aa19cd3085f653e51d949a4135d691
+Subproject commit 2772822d69aa19cd3085f653e51d949a4135d691-dirty
diff --git a/Koi.Prim2D b/Koi.Prim2D
--- a/Koi.Prim2D
+++ b/Koi.Prim2D
@@ -1 +1 @@
-Subproject commit 04ebec2dd37fd830067f0c4f3ccfae58f5c681b7
+Subproject commit 04ebec2dd37fd830067f0c4f3ccfae58f5c681b7-dirty
Entering 'Koi'
diff --git a/Koi/MyMath.cs b/Koi/MyMath.cs
index 64cacc6..f7fe636 100644
--- a/Koi/MyMath.cs
+++ b/Koi/MyMath.cs
@@ -24,7 +24,7 @@ namespace Koi
                 result = max;

             return result;
-        }
+        }   // end of Clamp()

         public static float Lerp(float a, float b, float t)
         {
Entering 'Koi.Prim2D'
diff --git a/Koi.Prim2D/Koi.Prim2D.csproj b/Koi.Prim2D/Koi.Prim2D.csproj
index 468930a..9e4f8ec 100644
--- a/Koi.Prim2D/Koi.Prim2D.csproj
+++ b/Koi.Prim2D/Koi.Prim2D.csproj
@@ -9,4 +9,8 @@
     <Folder Include="Painters\" />
   </ItemGroup>

+  <ItemGroup>
+    <ProjectReference Include="..\..\Koi\Koi\Koi.csproj" />
+  </ItemGroup>
+
 </Project>
```
The first part just shows the **-dirty** indicator which we see in GitHub Desktop.  The rests shows the changes, ie a comment has been added to MyMath.cs and Koi.Prim2D now references the Koi project.

## Getting Changes from Upstream
$ git fetch<br>
$ git merge origin/main

$ git submodule update --remote {Submodule Name}
$ git commit ????? Text talks about committing but doesn't show it.


## Pulling Changes from Local to Upstream


