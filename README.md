0. Restart from scratch!
No no no! We are already too far in the project to restart everything.

But once again, let’s work on a new codebase.

For this project you will fork this codebase:

Update the repository name to AirBnB_clone_v3
Update the README.md:
Add yourself as an author of the project
Add new information about your new contribution
Make it better!
If you’re the owner of this codebase, create a new repository called AirBnB_clone_v3 and copy over all files from AirBnB_clone_v2
1. Never fail!
Since the beginning we’ve been using the unittest module, but do you know why unittests are so important? Because when you add a new feature, you refactor a piece of code, etc… you want to be sure you didn’t break anything.

At Holberton, we have a lot of tests, and they all pass! Just for the Intranet itself, there are:

5,213 assertions (as of 08/20/2018)
13,061 assertions (as of 01/25/2021)
The following requirements must be met for your project:

all current tests must pass (don’t delete them…)
add new tests as much as you can (tests are mandatory for some tasks)
.
.
.
12. HTTP access control (CORS)
A resource makes a cross-origin HTTP request when it requests a resource from a different domain, or port, than the one the first resource itself serves.

Read the full definition here

Why do we need this?

Because you will soon start allowing a web client to make requests your API. If your API doesn’t have a correct CORS setup, your web client won’t be able to access your data.

With Flask, it’s really easy, you will use the class CORS of the module flask_cors.

How to install it: $ pip3 install flask_cors

Update api/v1/app.py to create a CORS instance allowing: /* for 0.0.0.0

You will update it later when you will deploy your API to production.

Now you can see this HTTP Response Header: < Access-Control-Allow-Origin: 0.0.0.0
.
.
.
15. Search
For the moment, the only way to list Place objects is via GET /api/v1/cities/<city_id>/places.

Good, but not enough…

Update api/v1/views/places.py to add a new endpoint: POST /api/v1/places_search that retrieves all Place objects depending of the JSON in the body of the request.

The JSON can contain 3 optional keys:

states: list of State ids
cities: list of City ids
amenities: list of Amenity ids

## Authors
 Aziza Aynaou - [Github](https://github.com/Azizaazu)
 boutaina RHAZOUI - [Github](https://github.com/boutaina96)
## License
Public Domain. No copy write protection. 
