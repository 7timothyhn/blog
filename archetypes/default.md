--- 
title: "{{ replace .Name "-" " " | title }}" # this page acts as the default look for the entire webpage.
                                            # and initiallized the perameters of each file
                                            # the title of each page will be set as the header when a file is selected or entered. 
date: {{ .Date }}  #the date will change based on the date inside each file
tags: []  # this is were the tages will be.
featured_image: ""  #this is were each image will be
description: ""  #this is where the desrciption will be
---

