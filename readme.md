# Tampa Devs

[![Netlify Status](https://api.netlify.com/api/v1/badges/3f72138e-3b19-4c34-99a8-6dfcb2bd6d82/deploy-status)](https://app.netlify.com/sites/tampadevs/deploys)


<!-- ## Editing the events

Events are stored in `src/_data/events.json`

Add new events at the top in the format:

```
  {
    "name": "Meetup",
    "date": "2018-10-18",
    "url": "https://eventbrite.com/…",
    "description": "This is an event description"
  },
``` -->

## Adding people

People are stored in `src/_data/people.json`

Add a new person with the format:

```
  {
    "name": "John Smith",
    "team": ["Team Member"],
    "img": "john.jpg",
    "bio": "John looks after developers in Florida."
  },
```

Avatars should be saved to `src/_assets/img/people`

## Development

To get this up and running on your own computer you need to have Node and NPM installed. [Find out how here](https://www.npmjs.com/get-npm).

Once you have installed NPM in the command line run the following line in this folder:

- `npm install`
- `npm run dev`

You'll now have a local server running at [http://localhost:8080](http://localhost:8080).

This is built on top of [Eleventy](https://www.11ty.io) because it is great. One of the nice things about 11ty is it's [super simple documentation](https://www.11ty.io/docs/).

Behind the scenes Webpack is handling JS (`src/_assets/_js`) and SCSS (`src/_assets/_scss`).

## Deploy

Pushing to `master` will automagically deploy to Netlify, which spits out the site at [tampadevs.com](https://tampadevs.com).

However if you want to test something… `npm run build` is your friend.

## TODO

- Google analytics is using the old UA functionality, needs to be ported to new setup. See how `basics.json` is consuming the tag analytic ID