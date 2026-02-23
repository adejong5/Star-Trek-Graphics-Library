# Star Trek Graphics Library
Library of graphical assets for creating Star Trek style images and svgs

> [!Important]
> This is very much a work in progress. Very few of the standards and conventions have actually been applied. Use at your own peril, and please contribute by creating a PR.

# How to use this library
This library is a collection of Star Trek themed images, svgs, and graphical assets. These are organized in categories using folders. Here is a not-up-to-date example:

```
├── MSDs  - Completed images for Master System Display 
│   ├── USS Enterprise NCC-1701.svg
│   ├── USS Enterprise NCC-1701.webp
│   ├── USS Enterprise NCC-1701-A.svg
│   ├── USS Enterprise NCC-1701-B.svg
│   ├── Deep Space Nine Plan View.svg
│   ├── Deep Space Nine Elevation View.svg
├── Assets  - Individual components which can be easily inserted into new designs
│   ├── People
│   │   ├── silhouette 1.svg
│   │   ├── silhouette 2.svg
│   ├── Arrays
│   │   ├── Nacelle 1.svg
│   │   ├── Nacelle 2.svg
│   ├── Engines
│   │   ├── Shuttle Engine 1.svg
│   │   ├── Car Engine 1.svg
│   │   ├── Car Engine 2.svg
│   ├── Wheels
│   │   ├── Wheel 1.svg
│   │   ├── Wheel 2.svg
├── Color Palettes  - Markdown documentation of common color palettes
│   ├── Next Generation Navigation.md
│   ├── Next Generation Engineering.md
│   ├── Voyager.md
│   ├── Deep Space Nine.md
```

- MSDs
  These are high quality, detailed images and SVGs for use in Master System Displays. These should follow the [Element Naming Convention](#element-naming-convention) whenever possible to facilitate in locating callouts.
- Assets
  These are individual components and pieces, typically taken from MSDs, which can easily be copy/pasted into new designs. These should be categorized by the physical description of the assets (e.g. "arrays" instead of "warp field generator bank") because they might be reused in other ways (e.g. an array of EV batteries"). These should follow the [Element Naming Convention](#element-naming-convention) whenever possible to facilitate in locating callouts.
- Color Palettes
  These are collections of common color codes from various eras, ships, cultures, and command functions.

# Element Naming Convention
Many Master System Displays include callouts pointing to key areas of the ship. To facilitate in creating these, elements can be given meaningful names. An obvious candidate for storing this information in an svg is using an `id` attribute. However, this is complicated by the fact that Inkscape automatically creates `id` attributes for every element, usually with meaningless names such as `path1234-2-1`. For this reason, both the `id` attribute and `Title` sub-element should be used. Examples include:
`<path id="Front Window" ... ><title>Front Window</title></path>` 
  for the `path` element containing the front window of shuttlecraft

```
<circle id="Engine Node 1" ...><title>Engine Node 1</title></circle>
<circle id="Engine Node 2" ...><title>Engine Node 2</title></circle>
<circle id="Engine Node 3" ...><title>Engine Node 3</title></circle>
```
for an array of nodes located in the engine compartment.

# Disclaimer & Affiliation
This project is a non-commercial fan production. *Star Trek* and all related marks, logos, and characters are solely owned by CBS Studios Inc. This fan production is not endorsed by, sponsored by, nor affiliated with CBS, Paramount Pictures, or any other *Star Trek* franchise. 

No commercial exhibition or distribution is permitted. No alleged independent rights will be asserted against CBS or Paramount Pictures. This work is intended for personal and recreational use only.

All attributions to other creators are embedded as metadata in each asset.