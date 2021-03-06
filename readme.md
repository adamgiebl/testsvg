<a href="#">
  <img src="header.svg">
</a>
<br />
<br/>

A small command-line tool that turns GLTF assets into declarative and re-usable [react-three-fiber](https://github.com/pmndrs/react-three-fiber) JSX components. See it in action here: https://github.com/drcmda/floating-shoe

The usual GLTF workflow is cumbersome: objects can only be found by traversal, changes are made by mutation, making contents conditional is hard. Gltfjsx creates a nested graph of all the objects and materials inside your asset, it will not touch or modify your files in any way. Now you can easily make the data dynamic, alter contents, add events, etc.

## Usage

```bash
Usage
  npx gltfjsx [path/to/model.gltf] [options]

Options
  --types, -t      Add Typescript definitions
  --verbose, -v    Verbose output w/ names and empty groups
  --meta, -m       Include metadata (as userData)
  --precision, -p  Number of fractional digits (default: 2)
  --draco, -d      Draco binary path
  --root, -r       Sets directory from which .gltf file is served

Examples
  npx gltfjsx model.glb -t
```
