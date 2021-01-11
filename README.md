# e-Template

### Purpose and Functionality

e-Template will

- make it easy for activists to find email templates applicable to the causes they want to support.
- make it easy for activists with or without a tech background to make customizable email templates.
- allow authors to see insights as to how much reach their published templates have had.

### To View on Heroku:

- https://e-template.herokuapp.com/

### To Run Locally:

- Frontend access the website at: [localhost:3000](http://localhost:3000)
- Backend access the website at: [localhost:8080](http://localhost:8080)

#### How to get heroku environment config vars for the database

Initialize this repo with heroku's git. You must be a collaborator and signed in on heroku for the e-template account to do this:

```
heroku git:remote -a e-template
```

there is a script called `get_env_from_heroku.sh` in `root/`.

```
npm install
chmod a+x get_env_from_heroku.sh
./get_env_from_heroku.sh
```

#### Frontend Only

- if you only want to look at the front end, you can try:

```
cd client
npm install
npm run start
```

#### Frontend and Backend

- if you want to test front and back end together locally, open two terminal windows one in `client/` folder and one in `root/` directory.
- Run the following in the `root/`:

```
npm install
npm run demon
```

- Run the following in `client/`:

```
cd client
npm install
npm run start
```

#### Production Build

- if you want to run it like heroku does (production build, will be slow to build)

```
npm install; cd client; npm install; npm run build; cd ..; npm start
```
