# Ah-Counter for Toastmasters

This is a simple Ah-Counter for my activities in Toastmasters.

## Get started

Install the dependencies...

```bash
git clone https://github.com/Spansky/ah-counter.git
cd ah-counter
npm install
```

...then start...

```bash
npm run dev
```

Navigate to [localhost:5000](http://localhost:5000). You should see your app running. 

To create an optimised version of the app:

```bash
npm run build
```

You can run the newly built app with `npm run start`. This uses [sirv](https://github.com/lukeed/sirv), which is included in your package.json's `dependencies` so that the app will work when you deploy to platforms like [Heroku](https://heroku.com).