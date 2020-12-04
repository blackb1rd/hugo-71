# outputFormats path issue for sections

This repository is a minimal case for showing how Hugo does not handle the `path` config for an outputFormat consistently across page types. For the home page and other pages, the path is set correctly to place the custom output in the `public/htmlcontent` directory. So the following are saved where I expect them to be:

- Index file: `public/htmlcontent/htmlcontent.html`
- Content page: `public/htmlcontent/basics/content/htmlcontent.html`

For a section/chapter the custom output is saved within the section like `public/basics/htmlcontent/htmlcontent.html`. I would expect that the section in this case would be in `public/htmlcontent/basics/htmlcontent.html`.

# image is not copied with Multilingual Mode and Custom output format
see

  -  Custom output format: `public/htmlcontent/cat-behaviour.jpg`
  -  Multilingual Mode + Custom output format: `public/th/htmlcontent/cat-behaviour.jpg` << no image found
