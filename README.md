# Reaction App

## DataBase Setup

1. Create mongoDB account - https://account.mongodb.com/account/register
2. Create AWS cluster
3. Under Security tab, click Database Access, and on the right `add new database user`. After you enter username and password, click `add user` at the bottom right corner.
4. Under Security tab, click Network Access, and whitelist your IP address.
5. Once your cluster is created, under Clusters tab, click connect and copy the connection string which will look something like this `mongodb+srv://<username>:<password>@cluster0.ioku4.mongodb.net/myFirstDatabase?retryWrites=true&w=majority`. Instead of `<username>` there will be your username, and you will need to replace `<password>` with your password.
6. Finally, inside your project folder, `cd` into server, create new file `.env` and enter `DB=<paste the string from above here>`. It will look similar to this `DB=mongodb+srv://srdjan:mypass@cluster0.ioku4.mongodb.net/reaction?retryWrites=true&w=majority`.

## Running the app
While in the server directory, run `npm run dev` to start the live server. The live server will watch for changes to files in the `src` directory and reload the page when they're changed.

## Viewing Static Version of the App
While developing the app, you can take a look at the static pages that you'll eventually convert into a dynamic application. To do so, visit `http://localhost:3000/ui` in the browser.
