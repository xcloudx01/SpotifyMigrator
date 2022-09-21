# Spotify Migrator
Spotify Migrator is an application to transfer your spotify data from an account to another
I never found an online service who did what I wanted, so I made this.
### If you find it useful, make sure to star Thank you!.

## Features

-  [x] Transfer your liked songs in order
-  [x] Transfer your playlists
-  [x] Create a copy of your playlists (make the new account owner)
-  [x] Follow your playlists
-  [ ] Follow artists/users
-  [ ] Add you to your collaborative playlists
-  [ ] Mark your collaborative playlist as collaborative instead of only public/private
-  [ ] Save Podcasts
## V1
You can still use V1 of Spotify Migrator(its a branch) if you want to, but I wouldnt recommend it, this project is meant to be evolutive and get better everytime I get bored.
## Installation

This application requires [Node.js](https://nodejs.org/) v10+ to run.

Run cmd or Terminal and navigate to where you un-zipped this repo.
Run this command to install all dependancies:
```sh
npm i
```

## How to use
To use this app you will need to create an app on the [Spotify Developer Website](https://developer.spotify.com/dashboard/applications)

Once you created your application, we will need to edit some informations.
#### Setting up the application
1. Click on "Edit Settings"
2. Go to RedirectURI and add the values:
- http://localhost:3000/callback  
![Image to Explain Step 2](https://raw.githubusercontent.com/JustSxm/SpotifyMigrator/master/meta/redirect.PNG)
3. Save  
![Image to Explain Step 3](https://raw.githubusercontent.com/JustSxm/SpotifyMigrator/master/meta/Save.PNG)
4. Go to Users and Access  
![Image to Explain Step 4](https://raw.githubusercontent.com/JustSxm/SpotifyMigrator/master/meta/UserAndAccess.PNG)
5. Add the email of the other account you are not currently logged in (new or old) to give it access to the application.

#### Setting up the config
Go back to the developer dashboard, click on the app you made, grab the Client ID and the Client Secret and put them in the file config.json (replace CHANGEME).

#### Start the app
Run cmd or Terminal and navigate to where you un-zipped this repo.
Run this command:
```sh
start "" http://localhost:3000 & node app.js
```
The app will start and it's interface will open in a web browser.

## Development
Want to contribute? Great!
There is multiple user-friendly things to add that I won't bother add that anyone could do.

- [x] CSS / Prettier pages
- [ ] Wait page while requests are being sent
- [ ] Reduce the time every second.


## License
GPL
