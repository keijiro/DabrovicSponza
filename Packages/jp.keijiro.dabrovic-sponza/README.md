Dabrovic Sponza
===============

![screenshot](http://i.imgur.com/stPvCV7.png)

**Dabrovic Sponza** is a Unity package containing the "Dabrovic Sponza"
architectural model, which the computer graphics community frequently used as a
test model.

Marko Dabrovic created the original model. Kenzie Lamar at Vicarious Visions
converted the 3DS file to OBJ and assigned texture coordinates to the ceilings.
Morgan McGuire hand-painted bump maps for most surfaces.

You can obtain the original model from the following page:

http://hdri.cgtechniques.com/~sponza/files/

Also you can obtain the refined model from McGuire's archive:

https://casual-effects.com/data/

How To Install
--------------

The Dabrovic Sponza package uses the [scoped registry] feature to import
dependent packages. Please add the following sections to the package manifest
file (`Packages/manifest.json`).

To the `scopedRegistries` section:

```
{
  "name": "Keijiro",
  "url": "https://registry.npmjs.com",
  "scopes": [ "jp.keijiro" ]
}
```

To the `dependencies` section:

```
"jp.keijiro.dabrovic-sponza": "1.0.0"
```

After changes, the manifest file should look like below:

```
{
  "scopedRegistries": [
    {
      "name": "Keijiro",
      "url": "https://registry.npmjs.com",
      "scopes": [ "jp.keijiro" ]
    }
  ],
  "dependencies": {
    "jp.keijiro.dabrovic-sponza": "1.0.0",
    ...
```

[scoped registry]: https://docs.unity3d.com/Manual/upm-scoped.html
