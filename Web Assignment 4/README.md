# Registration-sql

# [Complete user registration system using PHP and MySQL database |
complete-user-registration-system-using-php-and-mysql-database) | [YouTube video](https://www.youtube.com/watch?v=C--mu07uhQw)
In this tutorial, I walk you through the complete process of creating a user registration system where users can create an account by providing username, email and password, login and logout using PHP and MySQL. I will also show you how you can make some pages accessible only to logged in users. Any other user not logged in will not be able to access the page.

The first thing we'll need to do is set up our database. 

Create a database called **registration**. In the **registration** database, add a table called **users**. The users table will take the following four fields.

-   id
-   username  -  varchar(100)
-   email  -  varchar(100)
-   password  -  varchar(100)

You can create this using a MySQL client like PHPMyAdmin.



Or you can create it on the MySQL prompt using the following SQL script:

```mysql
    CREATE TABLE `users` (
      `id` int(11) NOT NULL AUTO_INCREMENT PRIMARY KEY,
      `username` varchar(100) NOT NULL,
      `email` varchar(100) NOT NULL,
      `password` varchar(100) NOT NULL
    ) ENGINE=InnoDB DEFAULT CHARSET=latin1;
```

And that's it with the database. 

Now create a folder called **registration** in a directory accessible to our server. i.e create the folder inside htdocs (if you are using XAMPP server) or inside **www **(if you are using wampp server).

Inside the folder **registration, 


Open these files up in a text editor of your choice. Mine is Sublime Text 3.

### Registering a user
The first if statement checks if the user is already logged in. If they are not logged in, they will be redirected to the login page. Hence this page is accessible to only logged in users. If you'd like to make any page accessible only to logged in users, all you have to do is place this if statement at the top of the file.

The second if statement checks if the user has clicked the logout button. If yes, the system logs them out and redirects them back to the login page.

And that's it!

Now go on, customize it to suit your needs and build an awesome site. If you have any worries or anything you need to clarify, leave it in the comments below and help will come.

You can always support by sharing on social media or recommending my blog to your friends and colleagues.

Best regards :D

Sarbesh_yadav
* * *

### You might also like:

<!-- -   [How to create a blog in PHP and MySQL database] -->
