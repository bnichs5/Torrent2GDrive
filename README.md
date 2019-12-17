[![Torrent2GDrive](https://torrent2-gdrive.herokuapp.com/img/Torrent2Drive.0211de43.png)](https://torrent2-gdrive.herokuapp.com)



# Torrent2Drive

> A web application to download torrent directly to your Google Drive using Nodejs in backend and Vuejs in frontend.


# Installation

## Deploy to Local Machine

- Clone this repo to your local machine using `https://github.com/pawanpaudel93/Torrent2GDrive`
- Goto [Google Developer Console[](https://console.developers.google.com)](https://console.developers.google.com) and create OAuth credentials.
- Goto `Torrent2Drive/Torrent2Drive_server` folder and create `.env` file and view file `.env-example` for reference and paste the following with OAuth credentials in .env file.

  `GOOGLE_CLIENT_ID=paste client id here`

  `GOOGLE_CLIENT_SECRET=paste client secret here`

  `SECRET=Torrent2Drive@VueJS` 


- Goto `Torrent2Drive/Torrent2Drive_frontend` folder and create `.env` file and view file `.env-example` for reference and paste in .env file

  `VUE_APP_BASEURL=http://localhost:3000`
- Goto `Torrent2Drive` folder and open terminal and write the following command for the project setup:
(Make sure npm is installed!)

  > npm run local-build
- Then to run the app write write:
  > npm run start
- So if you update the app code and to build and start the app write:
  > npm run build

  > npm run start

### Deploy to Heroku

- Goto [Google Developer Console[](https://console.developers.google.com)](https://console.developers.google.com) and create OAuth credentials.
- Deploy to Heroku

     > [![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/pawanpaudel93/Torrent2GDrive)

- Add all the environment variables from `.env-example` of `Torrent2Drive_server` and `Torrent2Drive_frontend` to Heroku app `Config vars` and add value for all. For `SECRET` paste value `Torrent2Drive@VueJS` or any custom text.

   `GOOGLE_CLIENT_ID`

   `GOOGLE_CLIENT_SECRET`

   `SECRET`

- Set heroku `VUE_APP_BASEURL` environment variable to your heroku app URL. I have used `https://torrent2-gdrive.herokuapp.com`. So, use your own heroku URL. 
