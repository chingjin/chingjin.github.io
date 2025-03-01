# Install Hexo
Consult [official documentation](https://hexo.io/docs/#Installation) to install hexo. In general, it involves these steps sequentially:
1. Install `node.js` (see above link for more information)
2. Install hexo
    - `npm install hexo`
    - Set relative path: `echo 'PATH="$PATH:./node_modules/.bin"' >> ~/.profile`
3. Install all the node modules already included in the repo: `npm install`

# Add Contents
## Edit self introduction
1. Navigate to `themes/frame/config.yml`
2. Find the section `profile`
3. You can edit title, subtitle, body and image. Should be pretty straightforward.
4. The image is saved in `themes/frame/source`

## Add publications
Edit `source/publications/index.md`
The file follows basic `markdown` syntax.

## Add projects or talks
### Create new file
Run the following line in the command line to create new file:
`hexo new [title]`

This will create a markdown file `source/_posts/[title].md` and a folder `source/_posts/[title]/`

### Set up front matter
All below actions are down on `source/_posts/[title].md`

#### Title
Fill in the title you want.

#### Date
The date of your project or talk. It will be relevant on the order of the items showed. 

#### Categories
If it's for projects, add 
```markdown
categories:
- research projects
```
in the front matter
If it's for talks, add
```markdown
categories:
- talks
```
in the front matter

#### Tags
Fill in the tags to display keywords. It should look something like this
```markdown
tags:
    - tag1
    - tag2
```

#### Featured Image
If you want to add a featured image for this article:
1. Put the image in the folder `source/_posts/[title]/`
2. Add to the front matter
```markdown
featured_image: [title]/[image_file_name]
```

### Write contents
Contents should be filled after the front matter. Follow the basic `markdown` syntax to fill in the contents.