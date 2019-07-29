.. title: Change the data type dynamically in mongo
.. slug: mongo-change-data-type
.. date: 2019-07-29 12:00 UTC
.. tags: mongodb, data wrangling
.. category: Tips
.. description: How to change the data type of field when it contains 2 or more data types.


I'm using mongo DB to initially store data I scraped from the web. And like all
good projects, I realized that I was storing a date value as a string. I
corrected the code, but now I have a field that haves the values stored as a
string and date object.

.. code-block:: javascript

   use scraped_db

   var cursor = db.scraped_collection.find({'datePosted': {$type: 'string'}});
   while (cursor.hasNext()) {
       var doc = cursor.next();
       db.scraped_collection.update(
                { '_id': doc._id},
                { $set: {datePosted: new ISODate(doc.datePosted) } }
       )


Simple and straight forward.

Happy hacking.
