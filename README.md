# ossec.github.io

This site is built with Sphinx using the code base in ossec.github.io/_project.
To visit the finished website, go to http://ossec.github.io.  Most of the website
should remain the same over time except when we have in OSSEC releases or want to 
add a blog entry. After cloning or forking this repo, follow these instructions to 
revise the website content for downloads or blogs.  

## Updating the Downloads page

1. cd to _project/
1. Open the downloads.rst file
2. Make changes to links where necessary.
3. Run *make clean* then *make html*.
4. Open _project/_build/html/index.html in a browser to see the new website.
5. Repeat steps 2-4 as necessary until the Downloads page looks right.
6. Replace the ossec.github.io/downloads.html with _project/_build/html/downloads.html
7. Run *make clean*.
8. cd to the top level ossec.github.io
9. Push all the revisions to ossec.github.io.

## Adding a blog entry

1. cd _project/blog/posts
2. Create a file using the naming convention *YYYY-mm-dd-TITLE.rst* in the blog/posts directory.
3. Open this file in the editor of your choice.
4. Replace *TITLE* with the title of your blog.
5. Add a section at the top of the blog file that looks like this:
   <pre>
       .. post:: MMM DD, YYYY
           :tags: your tags
           :category: your categories
           :author: your name

       =====
       TITLE
       =====
   </pre>
6.  Replace MMM with the month abbreviation of your blog, e.g. Jan, Feb, etc.
7.  Replace DD with the day number, e.g. 01, 02, 03, 3tc.
8.  Replace YYYY with the year. Note for steps 4-6 check the files in blob/posts for examples.
8.  Fill in the *your tags*, *your categories* and *your name* sections.  
9.  Write the blog content below your TITLE section.
10. cd to _project/  
11. Run *make clean* then *make html*.
12. Open _project/_build/html/index.html in a browser to see the new website.
13. Repeat steps 7-10 until your blog content looks right.
14. Replace ossec.github.io/blog.html with _project/_build/html/_blog.html.
15. Copy the HTML version of your blog from _project/_build/html/blog/posts to ossec.github.io/blog/posts/.
16. Run *make clean*.
17. cd to the top level ossec.github.io
18. Push all the revisions to ossec.github.io.
