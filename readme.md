![StorybookImg](https://github.com/StewedDownSteve/storybookscopy/blob/master/storybooksscreenShot.png)

# Storybooks Web App copy
A full-stack web app, copy of Storybooks format and function. Allows user to log in using google and post and share their own stories.



# How It's Made:
This app uses Node.js/Express/MongoDB/ Handlebars with Google OAuth for authentication. 

This helped tie in all my knowledge of Node, Express, and Mongo. Learning how to implement Google OAuth was much easier than originally expected. I got more familiar with Handlebars for forms and page layout.

# Optimizations

If I were to go back I would fix a few errors due to an updated version of Mongoose. One is around the Authentication section of the video: 'MongooseError: Model.findById() no longer accepts a callback'. I had success changing the code to deserializeUser at the end of passport.js to:

passport.deserializeUser(async (id, done) => {
        done(null, await User.findById(id))
    })
For fun, I would add as many authentications as I could, like Snapchat, Facebook, Twitter, LinkedIn, etc.
  

# Lessons Learned:
Honestly, this was a huge win for me. Tying together all my knowledge to make a full-stack app with authentication that actually can run made me feel like my back-end skills are growing. I have a lot to learn but I'm excited to make more apps like this and put my spin on them.
