<p align="center">
  <img width="auto" height="150" src="public/images/Logo copy.png">
</p>

# cReddit

This project was built using React, Ruby on Rails, PostgresQL, Semantic UI, React Router and Formik. This project was the culmination of Andrew Santos and I's progress through Mod4 at the Flatiron School. Over the course of the bootcamp, we have learned Ruby, Ruby on Rails, Javascript and React. The objective of the Mod4 project was to combine our knowledge of backend framework's like Ruby on Rails with the blazing fast speed of a React frontend.

### Our Objective

Andrew and I decided to create a mock "Reddit" with some added features. Our first extended feature was a "User Credibility Score." When a user creates an account, they are dropped into the cReddit community with 100 points. Our second added feature was for the user to claim their rebuttal to a post was either an opinion or fact. This led to another idea, if the user was claiming their response to a post as fact, they would have to add a url to a source that validates their claim. Our third feature was creating a Source Validation feature. Other users viewing a post and its responses would be able to either validate another user's rebuttal if it was a fact or dispute it. If the response's URL source provided insufficient evidence to validate the user's claim, other users can dispute the source, and so called fact, leading to decrementing the comment owner's credibility score. Vice versa, if the user provides a solid source for a rebuttal, the other users can validate, in turn, incrementing the user's credibility score. We then added a filter to sort posts and commments.

### Links to Repo's

Backend =>  <a href="https://github.com/TylerKnvpp/cReddit-backend">Ruby on Rails Backend</a>

Frontend => <a href="https://github.com/asantos649/cReddit-frontend">React Frontend</a>

### Challenges

##### Frontend

This turned out to be a fairly large project for only working on it for 4 1/2 days. We we're expecting to run into some roadblocks since we were using pure React without a state management library like Redux, but managing the data from the frontend went rather smoothly. We used this project as an opportunity to play with some React libraries such as Formik which made life really easy and added some nice field validations. Semantic UI was another library we used to fast-forward some the design of the project. It was straightforward to use and really helped dive our project a professional and clean UX. We did run into a problem with managing state with the built in forms which led us to Formik, but other than that it was really nice to work with Semantic.

##### Backend & Data Model

Rails was a pleasure to work with (at first). We spun up a backend, db and connected it to our frontend within an hour. We used the Rails API with a PostgreSQL database, bcrypt to ensure the user's password was encrypted end-to-end and serializer because our data models required nested objects. Our biggest challenge came from working with nested data. In certain scenarios, like updating a user's credibility score, we would find that the user object would drop off somewhere within our HTTP POST request. Each data model had each data model nested within it. A user object had an array of objects for Posts and an array of objects for comments. Comments had a user object that it belonged to and post object that it belonged to. Somewhere between our Frontend and Backend the object would be lost and typically replaced with an id corresponding to a post or user or comment. To combat this we hardcoded a solution in the backend to find the corresponding data and attach it to the POST request.

### Conclusion

This was a really fun project to work on. We gained solid experience in all that web development entails: wireframing, design, UX, data modeling, open-source libraries, backend + frontend techonologies and tying them together. We are proud to present this project and really enjoyed working on it.


