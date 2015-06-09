# Collaborating on the new Ricston (UK) Site Content For Geeks

To get a new Ricston UK site, checkout the following project in a folder of your choice

```
git clone https://github.com/ricston-git/ricston_site.git
```

This will check out a static website based on node **hexo**.

## Building and Run the Site Locally
1. Install [nodejs](https://nodejs.org/)  if you haven't  already
2. Install the [hexo](hexo.io) tool
```
npm install hexo-cli -g
```
3. Then inside your ricston-site folder run
```shell
hexo  generate
```

this will will publish the markdown pages in `source` to `public`

4. Run a server and test the sie is there
```
hexo server -p 5000
```

Navigate to http://localhost:5000  .. and go wow !!

## Creating Pages, Posts and making Changes from Locally

in your local version you can create a new blog post
```
hexo new "May awesome blog content"
```
This will create a markdown page on `My_awesome_blog_content.md` in the source/\_posts
directory. Using a simple text editor, your editor of course or  https://stackedit.io/,  http://atom.io  you can edit the markdown content

Do the ```hexo generate`` and view on the ``hexo server```

Static pages can be created in the same way by adding to the source diretory with a directory of your choice


Using the wonder of git you can
* ```git add``` your new pages
* ```git commit```  your changes with a reason for the change
* ```git push``` to the main repo

where the changes can be pulled, reviewed and published

## Making Quick Changes from Git repo
Any pages in the git repo can be quickly edited form the github website
and the same publish process is followed

## Pulling your other repo's and personal gists ..
Git pull and build

## Links and References
* http://hexo.io
* https://help.github.com/articles/github-flavored-markdown/
