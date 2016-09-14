When ProfilePress is [installed and activated](../installation.md), the custom pages it create for login, registration and password reset are automatically set as WordPress default. Thus when a users visit the following URLs:


* http://yoursite.com/wp-login.php
* http://yoursite.com/wp-login.php?action=register
* http://profilepress.net/wp-login.php?action=lostpassword


They will be redirect to the page containing the custom login, registration and password reset form created by ProfilePress.


**An example:** click [http://profilepress.net/wp-login.php](http://profilepress.net/wp-login.php) and you will be redirected to the website custom login page.


To alter these pages settings, click the **Settings** ProfilePress menu and go to the `Global Settings` section.

![Redirect WordPress login, registration, password reset page to custom page](https://profilepress-523b.kxcdn.com/wp-content/uploads/2015/01/make-custom-pages-default.png)


## User Redirections

To redirect users to a custom page or URL after they log in and log out, select the pages or enter the URL in `Redirection` section and save.

![Login, logout and edit-profile redirect](img/user-redirection.png)

**Note:** URL entered into the custom URL field takes precedence over a selected page.

If you've created a custom [edit profile page](../build/edit-profile.md) and want users to be redirected to the page when they click the `Your Profile` link in WordPress dashboard, check the activate checkbox of **Edit User Profile**.

![WordPress default profile link](img/wp-default-profile.png)


## Custom Redirections

Starting from version 1.1.0, custom redirect can now be set per login and registration shoortcodes via the `redirect` attribute.


For example, a custom login page with the shortcode  
`[profilepress-login id="2" redirect="http://xyz.com/welcome"]` will redirect users to the URL **http://xyz.com/welcome** after they are logged in.


Similarly, a registration page with the shortcode  
`[profilepress-registration redirect="http://xyz.com/welcome"]` will log users in and redirect them to the **http://xyz.com/welcome** after they successfully create an account.
