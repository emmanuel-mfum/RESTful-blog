# RESTful-blog
Blog as a Flask application that implements http routes that allow the user to create new blog posts, edit posts and delete posts.

This web blog stores the blog posts in a SQLite database (which contains the blog posts). The blog follows RESTful  principles since it is set up with HTTP routes that
follows the RESTful routing pattern as well as implementing routes for GET, POST, PUT and DELETE HTTP request verbs.

An interesting feature added in this blog prototype is the use of the CKEditorField in order to save the body of the post as HTML. 
The CKEditorField allows us to make things bold, add images and links, paste formatted text, etc. 
It's marked up and stored as HTML so that it can be rendered on our web pages (the blog in this case) with the formatting and images you used to write it. 
Otherwise, it would be just a plain boring text block.

In order to avoid rendering the HTML contained in the body of text of the blog post, we need to use a Jinja filter ,safe() in the "post.html" file
Overall, this project was a good practice in implementing Flask routes and passing parameters to the rendered HTML pages or to the Flask server.

Homepage:

![image](https://user-images.githubusercontent.com/55893421/116823859-ec993c00-ab54-11eb-9faa-bddb6c0c14ad.png)

Making a new post

![image](https://user-images.githubusercontent.com/55893421/116823890-22d6bb80-ab55-11eb-90e7-b6acb098b0d2.png)

![image](https://user-images.githubusercontent.com/55893421/116823897-2f5b1400-ab55-11eb-81cd-e7c5f25d02d4.png)

Editing an existing post

![image](https://user-images.githubusercontent.com/55893421/116823913-4568d480-ab55-11eb-93e1-e86b375a80ed.png)

![image](https://user-images.githubusercontent.com/55893421/116823923-51549680-ab55-11eb-9b72-80ca49b64140.png)

