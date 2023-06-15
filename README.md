# This file include the instructions I followed and what I did to get the code working

The first step is to brain storm the content of the blog and write down key points. 
Specifically a the title, the content of the blog and the images for each post and 
images for any other item. In this case, the theme Ananke uses a baground image for 
the top page.

The quick start page is the first step to using the hugo. https://gohugo.io/getting-started/quick-start/
Then follow the instructions and all the installations that are required. In my case,
were:
- Powershell
- Hugo
- choloatey 
- Go

Then, inside the powershell terminal in administrator mode, I created a file and called 
it blog, then coppied and pasted the first section in the hugo tutorial.

`hugo new site quickstart` // this creates a file that has all the hugo realted files 
    to get started
`cd quickstart`
`git init`
`git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke themes/ananke` 
    // this gets the theme and all the infroamtion reated to the theme, in this case 
    Ananke and saves it as a file called themes. This themes file also contains the 
    information needed to run the theme as well as the README instructions to use the
    the theme as well as the examplesite file which is what we care about the most.
`echo "theme = 'ananke'" >> hugo.toml` // this adds the theme to the hugo.toml file,
    which is another important file that will contain the primary code to run the
    code.
`hugo server` // this code is used when ever the you want to test to see if the 
    hugo code works and how your site looks.

# getting started

The three main files of importance is the 
`archetypes` folder // will hold the default.md file and which will hold all the 
    nessecary fields that each post or each mark down(.md) field will have. This
    file can be coppied from the theme file and pasted into the archetypes folder
    and that is it. 

`content` folder // this is where all the content and infor mation goes. in the example 
    folder they have two languages fr and en but you can ca copy and passed the en folder
    to your content folder. After you do that then things start to change between themes. 
    In the en folder, there are two files and two folders. The about folder will contain 
    the about page, the posts will contain all the blog posts and the title page off the 
    posts section, _index.md is the main file and will house the home page content and 
    contact.md is the file that has the contact page.
    
`hugo.toml` file // This file contains the general hugo toml data and has all the basic 
    the basic data that you will need in the first four lines. This file can also be coppied
    from the config.toml file in the examplesite file in themes. although the although the 
    only part that is needed is the english section and any other perameters that you want to
    add from the param field and that is it.

`static\images` a folder that is not automatically downloaded but is required if you want to 
    upload an image. This folder is called on when you want to generate an image using the
    key words `featured_image: "/images/ ----name of the jpg file goes here---- "`. the
    location of the image on the website is also dependent on the theme. 

    
The each all three files have been decomented to the best of my knowledge.

