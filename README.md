# Faces of Microsoft Open Source Contributions

## Project: Identify All the People!

There are 3,078 GitHub avatars in this picture. Each one is a Microsoft open source contributor. Let's see how many of these we can tie back to their GitHub profile page.

[Look at the image](https://patridge.github.io/msft-oss-contrib-img-dissect/). If you see someone you know who isn't already identified, let's get them added.

## See Someone You Know?

If you recognize someone who isn't already identified, just click the link for their picture and it will take you to the line to edit. That's right, the kludgy script file I put together has a line for every cell.

At the line for the desired cell, replace the `null` part of that cell's `github: null` portion with their GitHub username as a string.

For example, if you clicked an image cell and ended up seeing this line.

> `{ x: 15, y: 3, github: null },`

You would edit it to this, using the GitHub username you know for that cell.

> `{ x: 15, y: 3, github: "someoneawesome" },`

From there, just commit your changes to the branch GitHub will help you create and submit a pull request that we can merge in to update the links.

You should be able to do everything you need from the GitHub web editing system (though experiences may vary on mobile). While it is all written in JavaScript, you probably don't need to know it to make this work.

## Found a Mistake?

That happens. If you find someone who is incorrectly identified, you'll have to find the incorrect username in the [*script.js*](https://github.com/patridge/msft-oss-contrib-img-dissect/blob/master/script.js) file. From there, the process to commit and submit a pull request is the same.

## The Photo

This photo was put together to give a face to the many Microsoft contributors to open source software. It was [presented by Julia White at Red Hat Summit](https://twitter.com/julwhite), and a [full video of just the testimonials](https://youtu.be/4EYseGkkk_c) is also available.

I first saw this photo posted as a [tweet from OSCON3017](https://twitter.com/reid24hrs/status/862346968781271040) from [@reid24hrs](https://twitter.com/reid24hrs/). I asked if anyone had a better copy, and [Reid came through again](https://twitter.com/reid24hrs/status/862749470752215044).

After some back-and-forth, the original creator, [José Miguel Parrella](https://twitter.com/bureado/) [gave us permission to use it here](https://twitter.com/bureado/status/863071576421392384) (and even provided me with an even [larger version](original-github-avatar-collage.png) that was slightly reduced for web use).

## Run it yourself

This site is currently hosted from GitHub pages. If you want to, you can fork it, play around, and run it from your fork's GitHub pages system.

If, for some reason, you want to run this site locally, you'll need [Node.js](https://nodejs.org/). Once you have it, just run the following command.

> `node server.js`
