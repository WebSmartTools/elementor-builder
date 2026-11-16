# Transplant Checklist

Use this list every time you copy a section, column, or widget subtree from one Elementor JSON file into another.

## Before you copy

- [ ] You have the source file and the target file open.
- [ ] You know which subtree you are copying, top element down to its deepest child.
- [ ] You know the target site's media library IDs for every image in the subtree, or you have marked the file as needing them.

## Copy

- [ ] Copy the whole subtree verbatim, top element and everything nested under it.
- [ ] Do not regenerate any style ID. Do not rename any style label.
- [ ] If two elements in the target file now share an element ID, regenerate the copied element's ID and update any style ID derived from it in the same subtree. Keep the style label unchanged.

## Check the backgrounds

- [ ] Every `background` prop in the copied subtree matches the envelope in Rule 2 of SKILL.md.
- [ ] Every `image-attachment-id` exists in the target site's media library. Replace any that does not.
- [ ] The placeholder ID 12345 and the example.com URL from the skeleton file are replaced with real values, or the file is clearly marked as not ready to import.

## Check the classes

- [ ] Every `e-` class in the copied subtree exists in the same element's `styles` dict.
- [ ] Every `g-` class is noted. The target kit must define it, or the import will create a `DUP_` copy.
- [ ] No class in the file starts with `DUP_`. If one does, replace it with the plain class name before import.

## After import

- [ ] On each imported element, remove any `DUP_` class and add the plain class, in the editor.
- [ ] Test every click handler on the page.
- [ ] Check the page at desktop, tablet, and mobile widths.
- [ ] Check that the tablet breakpoint declares its own direction, gap, children width, and padding.
