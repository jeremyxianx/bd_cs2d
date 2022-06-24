Add a Book to the Database
--------------------------

.. http:: /libapi/book
   :noindex:
   
     Add a book written by a specified author.
	 
   :form string: author (*required*) -- The name the of the author of the book
   :form string: title (*required*) -- Title of the book
   :form string: publisher (*optional*) -- Publisher of the book 
   :form string: latest_publication_date (*optional*) -- Most recent publication date
   :form string: language (*optional*) -- Language used in the writing of the book 
   :form string: isbn10 (*required*) -- ISBN 10 number of the book
   :form string: isbn13 (*optional*) -- ISBN 13 number of the book
   
   :requestheader Authorization: `token`

**Example Request**

.. sourcecode:: bash
 

**Example Response**

.. sourcecode:: json

   {
       "result": "Timeline by Michael Crichton was added to the database"
   }
