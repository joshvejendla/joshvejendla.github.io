## Background

GitHub Pages is a service that allows you to host a free, low-code portfolio or blog directly from a git repository. It uses Jekyll, a static site generator, to automatically process YAML configuration files and Markdown text files into HTML web pages.

GitHub Pages allows you to use pre-made themes to implement your front-end without the need for custom code. It is also highly extensible, allowing for the inclusion of HTML, CSS, and Liquid (Jekyll's templating language) to further customize your front-end as you see fit.

## Setting Up Your Site

1. Start by creating a GitHub account here: https://github.com

2. Choose a theme that best suits your needs. 
	
	You can browse themes here: https://jekyllthemes.io, or by googling "jekyll themes", or by searching GitHub for "github pages themes". 
	
	Once you have found a theme that you like, go to the GitHub repository where the theme is hosted

	This website is built on using the Minimal Mistakes, which I will be using for the purpose of this article. It can be found here: https://github.com/mmistakes/minimal-mistakes

3. Fork your own version of the theme by clicking "Fork" at the top right of the page

   ![Minimal Mistakes Theme](/assets/images/Minimal Mistakes Theme.png)

4. Set the name of your repository version to \[USERNAME].github.io, replacing \[USERNAME] with the username you used to sign up with GitHub.

	GitHub Pages has a specific naming convention for the urls of its sites. My GitHub username is joshvejendla, so my GitHub Pages repo will be named joshvejendla.github.io

   ![Naming Your GitHub Pages Site](/assets/images/Naming Your GitHub Pages Site.png)

6. Host your GitHub Pages site by going to Settings > Code and Automation > Pages, then set the source to deploy from branch “master/root”
  
   ![GitHub Pages Settings](/assets/images/GitHub Pages Settings.png)

The build process for your site may take up to 10 minutes. To check if your site was hosted correctly, type your repository name (\[USERNAME].github.io) into your browser search bar. The site should be hosted with the starter template.

## Configuring Your Site

To start editing your site, go to the file \_config.yml and begin making your changes.

## Markdown Basics

# \# This is the largest heading (Heading 1) 
## \## This is a Heading 2
### \### This is a Heading 3
#### \#### This is a Heading 4
##### \##### This is a Heading 5
###### \###### This is a Heading 6

This is **\ **bold** \** text




