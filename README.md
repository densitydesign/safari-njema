# Safari Njema - Polisocial Award 2018
## Website available at: https://www.safari-njema.polimi.it/

To create a new research insight on the main page, add a new file called `question0X.markdown` in the `/_questions/` folder, where X is the number consequential to the other research outputs.

In the `/assets/images/` you can create a folder called `question0X` to store all images that you want to publish in the research output.

Meta tags (between the ---):
- number: from 1 to n, following the latest page. Each research insight comes after the other.
- permalink: if you want to customize the final URL of the output to have a easier-to-share link. It must be `structured-like-this`. **Remember that it's case sensitive**
- cover: the link to the cover image that will appear in the Outputs page. Put an image called `cover.jpg` in the folder `/assets/images/question0X/`
- layout: output. **Do not change this.**
- type: `visualization` or `post`. If a `visualization`, to add an image as visualization please contact Andrea. If `post`, no further action is needed.
- title: Title of your research output.
- sources: here you can list all additional materials that support the research output. They can be documents, datasets, external links. Each source is structured as follow:
  - name: the name of the resource.
    link: the URL where the resource is located. 

This is the template, copy and paste it in your new `question0X.markdown` file:

```
---
permalink: "/my-output/"
number: X
layout: output
cover: "/assets/images/question0X/cover.jpg"
type: post
title: Calculating and visualizing iso-chrone lines in Maputo
sources: 
- name: Dataset 1
  link: path/to/dataset/material
- name: Material 2
  link: path/to/dataset/material
---

Your research text. You can use markdown syntax available here: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
```

Right now, **the website is not automatically updated**. Contact Andrea if you plan to upload a new research output and he will upload the final results directly to the website https://www.safari-njema.polimi.it/.

## Further developments
- [ ] Automatic deploy from Github to FTP
