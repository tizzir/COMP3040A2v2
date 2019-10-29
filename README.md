# Hosting your resume online using GitHub Pages
## And how to keep it looking decent

Hosting your resume online is a great option if you're looking to share your
credentials quickly and to a large audience, while also saving paper. This
instruction set is designed to help you get your resume online using GitHub
Pages, a simple and efficient static site generator, and make it look pretty in
the process.

 > This guide is intended for audiences who are already familiar with Markdown
 > and Git. If you find that some of this guide is going over your head, you
 > might want to check out some info on [Git]() and [Markdown]().
 > 

## Prerequisites

Very little is required in order to complete this guide and have your resume
hosted online on a robust static website. You may take some of these things
for granted, but make sure you have them.

- A knowledge of Markdown
- A knowledge of Git
- A GitHub account
- Some method of accessing content on Git repos (Git CLI, GUI, GitHub online editor, whatever)

## Instructions

### Acquiring the template

In this guide we're going to start by using an existing template. This template
is what provides the format and look of the resume, and we'll simply dump our
own content into it. Every template is a little different, but here we will use
elipapa's [markdown-cv repo](https://github.com/elipapa/markdown-cv) template.
It looks nice and clean, and setting it up requires minimal fuss. The following
steps guide you through template acquisition.

1. Fork the [markdown-cv repo](https://github.com/elipapa/markdown-cv).
2. Optionally, change the name of the repo to something more specific or
   personal.
3. Clone the repo on your local machine.
4. Check out the `gh-pages` branch.  
     This branch is the one you want to be making all of your changes in. If
     you're having issues with GitHub pages displaying the latest changes
     later on, make sure the gh-pages branch has all of your latest changes,
     because it's the only branch that has any effect on deployed resume.

With these steps completed, you're ready to move onto the fun part of the
process, filling the resume with the content you want.

### Preparing your resume

Conveniently, a sample resume in the template's formatting is already provided,
so creating the resume is as easy as replacing the sample data with your own in
most cases. The steps below outline this process.

1. Open the sample resume `index.md` in the root of the repo.
2. Replace the sample contents with the contents of your own resume.  
     Note that not all Markdown markers work the same way in this template as
     they do in typical Markdown interpreters. Follow the markup patterns used
     in the sample template when adding your own content.  
     **Note**: ensure that the following code snippet remains at the top of
     `index.md`:
```
---
layout: cv
title: <Your resume webpage's title>
---
```

### Configuring the Repo

Once you've modified `index.md` to your liking, you need to push the
modifications and ensure the repo is properly configured display the content as
a static site using GitHub Pages.

1. Commit your personalized `index.md`.
2. Push the changes to your forked GitHub repo.
3. Ensure GitHub Pages is enabled for your forked repository
   1. Visit the webpage for your forked repository on GitHub pages
   2. Click the 'Settings' button underneath the project header.
   3. Scroll down (or `ctrl`-`f`) to the GitHub Pages section in the settings page.
   4. Ensure that the *Source* dropdown is set to the *gh-pages* branch, and that the *Theme Chooser* dropdown is blank (because these themes may interfere with the resume's template).

### Putting on the Final Touches

The final steps in this process involve viewing your resume as it is hosted,
making any fixes or modifications as necessary, and finally pushing
the resulting changes.

1. Go to `<your username>.github.io/<your forked branch's name>` to view your resume as GitHub displays it.
2. Proofread the resume, noting any issues you have with it.
3. If there are issues with the resume, return to editing the `index.md` file, fixing all issues you've noted.
4. Once you've solved the issues, commit the changes and push the changes
5. wait 1 - 3 minutes for GitHub to apply the changes to the static site, and then refresh the page to ensure that all of the changes have been fixed.  
    If there are still issues, repeat steps 3 to 5 of this section until all
    issues are resolved.

## FAQ

### **Can I use a theme/template/style other than `markdown-cv`?**  
Sure you can! Googling 'GitHub Pages resume template' will give you a bunch of
results featuring different templates compatible with GitHub pages.
Unfortunately, since each template may have a slightly different setup process,
dealing with all of the possible setup processes is out of the scope of this
document. Using the steps outlined in this document as a general guide for the
*flow* of using different templates would be a good starting point, though.

### **Can I still make use of `markdown-cv` without forking it? I don't want GitHub to prominently display the original repo to others who are looking at my resume.**  
While you absolutely can make use of `markdown-cv` without forking it on
GitHub, you'll still want to credit the original work somewhere. In this case,
consider adding an acknowledgment in your `README` file. Also, note that
because `markdown-cv` uses the MIT license, you'll also have to make your repo
use the MIT license. Always remember to pay attention to software licenses and
what each one allows and disallows before redistributing it.  
with that being said, note that you can just head over to the
[markdown-cv repo](https://github.com/elipapa/markdown-cv) and choose to
download the repo as a zip file. From there, you can make your modifications
and push all of the files to a new repo you create.

## Further Reading

This guide is just the tip of the iceberg when it comes to hosting your resume
or other documents online. If you're interested in digging deeper into the
systems at play in this guide, consider looking at some of the technologies
below.

| Technology | Description |
| -- | -- |
| [Jekyll](https://jekyllrb.com/) | Jekyll is the software the GitHub pages uses to display plain old Markdown files as aesthetically-pleasing static sites. Jekyll can be used locally to help preview changes as you make them. |
| [Sphinx](http://www.sphinx-doc.org/en/master/) and [ReStructuredText][(https://www.sphinx-doc.org/en/master/usage/restructuredtext/index.html) | Sphinx is a static site generator designed for displaying documentation and other text files in a nice format, like Jekyll. Sphinx, however, works with the ReStructuredText standard instead of Markdown. If you're interested in alternatives to what was used in this guide, it might be worth it to check out these technologies. |

## License

Everything included in this repo is licensed under the MIT software license.
See [`./LICENSE`](./LICENSE) for more information.

## Acknowledgments

I'd like that thank [elipapa](https://github.com/elipapa) for his
[markdown-cv](https://github.com/elipapa/markdown-cv) template. It's clean and
easy to dump your own information into, while still offering some flexibility.

Additionally, I'd like to thank [Enosh Anwar](https://github.com/EnoshAnwar)
and Louis O'connor for proofreading this readme.
