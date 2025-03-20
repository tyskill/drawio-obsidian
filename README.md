# Draw.io diagram plugin for Obsidian.md

This plugin introduces diagrams to Obsidian that can be included within notes or as stand-alone files. Diagrams are created as SVG files (although .drawio extensions are also supported).

![Screenshot](/docs/image/screenshot1.png)

## Usage
### Add / Insert a New Diagram

![Insert new diagram](/docs/image/screenshot2.png)

### Edit an Existing Diagram

![Edit existing diagram](/docs/image/screenshot3.png)

## Dev

### Compile

```bash
rollup --config rollup.config.js --bundleConfigAsCjs
```

### Upgrade Drawio

```bash
cd ./drawio
# pull remote tag
git fetch origin tag <tag_name>
# checkout tag
git checkout <tag_name>

# commit `upgrade` record
cd ../
git add drawio
git commit -m "Update drawio to tag vx.x.x"
```