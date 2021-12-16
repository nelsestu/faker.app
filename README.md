# faker.app
Generate fake data using Faker.js in a Node application. generated from [here](https://github.com/justusmbuvi/Faker.js-node-application)

## Steps

- Initialize project
- Configure nodemon in package.json
- Add a starting point
- Add models folder
- Add a views folder
- Start MongoDB
- Run the project

## Results
**Main Webpage**
![Main Webpage](fakedata-home.ejs-webpage.png?raw=true "Results Webpage")

View the steps in the webpage found [here](https://justusmbuvi.github.io/Faker.js-node-application/).

### Folder Structure
The folder structure will be as shown below:

Fakedata (Root Directory)

-- node_modules (folder)

-- models (folder)
  \
   -- user.js (file)

-- views (folder)
  \
   -- home.ejs (file)

-- app.js (file)

### How the project will run
The code when executed will use the faker.js library to generate the data needed several times. It will store each value generated in a local database. We shall then see the results in a web browser as a webpage from the database.

### Clone the repository
Clone this repository on your machine.

### Install the dependencies
The node libraries required for this tutorial include:

* nodemon
* express
* ejs
* mongoose
* faker

In the integrated terminal, run the following command to install the above packages all at once:

``` npm i nodemon express ejs mongoose faker ```

### Configuring package.json
Now open the “package.json” file and configure it so that you can start the application using nodemon. Under the scripts, add the “dev” and “start” configurations. The code should look as follows:

```
{
    "name": "fakedata",
    "version": "1.0.0",
    "description": "",
    "main": "app.js",
    "scripts": {
        "start": "node app.js",
        "dev": "nodemon app.js",
        "test": "echo \"Error: no test specified\" && exit 1"
    },
    "author": "",
    "license": "ISC",
    "dependencies": {
        "ejs": "^2.7.4",
        "express": "^4.17.1",
        "faker": "^4.1.0",
        "mongoose": "^5.12.5",
        "nodemon": "^2.0.7"
    }
}
```
### Run the project
Before running the code, make sure that MongoDB is running in the background.

In your integrated terminal, run the following command: ``` nodemon run dev ```
