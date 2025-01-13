---
type: assignment
date: 2025-01-15T08:00:00-5:00
title: 'Assignment #0 - How to submit assignments?'
thumbnail: /static_files/assignments/hw0/thumbnail.png
due_event:
    type: due
    date: 2025-01-27T23:59:00-5:00
    description: 'Assignment #0 due'
hide_from_announcments: true
---

## How to submit assignments? (in general) 
For each assignment, you will be required to submit two packages unless specified otherwise:  your __code__ and your __webpage__:
### Submit code to Gradescope
For every assignment you should create a `main.py` that can be used to run all your code for the assignment, and a `README.md` file that contains all required documentation. Place all source code used to generate your results, as well as any documentation required to use the code, in a folder named `andrewid_code_projX` where X is the hw number. Zip the whole folder and submit the zip to Gradescope. Here is an example of your folder structure:
```angular2html
zhiqiul_code_proj1/
    main.py
    README.md
    utils.py
    ....
## zip the whole folder to zhiqiul_code_proj1.zip:
```

### Submit your webpage to the class website
We will use [Andrew File System(AFS)](https://www.cmu.edu/computing/services/comm-collab/collaboration/afs/how-to/index.html) to store and display webpages. Here is a step by step tutorial: 
1. Place your website under folder `projX` and zip it. Please make sure that your main report page is called `index.html` so browsers open it automatically. X is the hw number.
2. Remote Copy. Use WinSCP or your favorite scp/ftp tool to copy all your files to your Andrew home directory `scp projX.zip andrew_id@linux.andrew.cmu.edu:/afs/andrew.cmu.edu/usr1/andrew_id/`.
3. Log in to a Unix Andrew machine: `ssh andrew_id@linux.andrew.cmu.edu`
4. File Transfer.  Unzip your website and copy the folder to your project directory: `cp -r projX/ /afs/andrew.cmu.edu/course/16/726-sp25/www/projects/andrew_id`.
   The folder structure should look like this:
    ```angular2html
    # suppose you are at /afs/andrew.cmu.edu/course/16/726-sp25/www/projects/andrew_id/
    index.html
    proj1/
        index.html
        data/...
    proj2/
        index.html
        data/...
    ```
5. Publish. The course website needs to be refreshed with your updated files. Do that by going [here](https://www.andrew.cmu.edu/server/publish.html), choosing web pages for a course, and inputing 16-726-sp25. With more files, this process may take a lot of time. So, please publish it only after you have transferred the final website.
6. Last step, test your page by visiting: `http://www.andrew.cmu.edu/course/16-726-sp25/projects/andrew_id/projX/`.

__FAQs__
- Remember __NOT to use any absolute links__ to images etc, as these will not work online. __Only use relative links.__\
- Note that 16, 726-sp25 is connected by `-` in URL while your folder is `16/726-sp25/`     
- Do not try using WinSCP/scp or similar to copy directly from your laptop to your class project directory as you don't have the credentials.
- Afs gets unhappy if your quota is full. Run `fs quota` to see the percent used; if it's close to 100 percent, delete things (java and matlab dumps, large tif's...) before trying the copy again.
- Your project directory is linked to your _Andrew_ id; if you use a CS computer (*.cs.cmu.edu), and run into trouble, try the instructions above, using an Andrew computer to hand in your work.
- If you have problems with images not appearing on your page, check that 1) filenames match your html files (e.g. .JPG vs .jpeg). 2) relative path is used from the correct root directory. 
- Please contact TA if there are problems. 


## What to submit for hw0?
Make sure you have tested the above steps and please:
- Change the `index.html` file created for you at `/afs/andrew.cmu.edu/course/16/726-sp25/www/projects/andrew_id/proj0/index.html`. Be creative!
- If you are not familar with html/css, this is a good time to start learning some of the basics. [w3schools](https://www.w3schools.com/html/default.asp) has some basic tutorials.