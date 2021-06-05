# Youtube-Model Migration With Sequelize

In this section I will put the record of how to implement Sequelize Migration into my node/express project.

At first, we have to follow this sequelize website when we will work.

here is the link: https://sequelize.org/

I am following that link and writing it in my own short way.

Things we need to do at first.

1. we have to make folder for mine `youtube-model`
2. into that project folder we need to run `npm init`
3. the install `npm install sequelize`
4. after that install database dependencies `npm install pg pg-hStore` I used postgres
5. install sequelize Cli `npm install --save-dev sequelize-cli`

Now Sequelize will structure our project by writting below command

1. `npx sequelize-cli init`

Now make the model for database table

2. `npx sequelize-cli model:generate --name User --attributes firstname:string, lastname:string, email:string`

by writing this command you will get the model and migration files into your project

3. finally after making all the relations on the table try to write
   `npx sequelize-cli db:migrate`

Check your database you will find your respected tables there.
