Express-Gallery
===============

MEH stack - Mongo Express and HTML5 

Use the MEH stack plus *almost* any other library or templating engines you want to fulfill the requirements.  
recommended: sass, jade, mongoose, bower, jQuery, foundation.  
helpful: livereload, gulp for watching compiling sass

---

Create a multi-user Gallery.  
Any user should be able to access these routes:  

- `GET /` to view a list of gallery photos
- `GET /gallery/:id` to see a single gallery photo
  - each gallery photo should include a link to delete this gallery photo
  - each gallery photo should include a link to edit this gallery photo
- `GET /new_photo` to see a "new photo" form
  - the form fields are:
    - `author` : Text
    - `link` : Text (the image url)
    - `description` : TextArea
- `POST /gallery` to create a new gallery photo i
- `GET /gallery/:id/edit` to see a form to *edit* a gallery photo identified by the `:id` param
  - the form fields are:
    - `author` : Text
    - `link` : Text (the image url)
    - `description` : TextArea
- `PUT /gallery/:id` updates a single gallery photo identified by the `:id` param
- `DELETE /gallery/:id` to delete a single gallery photo identified by the `:id` param

---

Your app should be stored in subdirectory `/app`.  
The layout of the app must match the layouts included in `/layouts`.  
Match the layout as close as you can, using free and open fonts and graphics.