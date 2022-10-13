# url4short

URL shortener with PHP and PostgreSQL

  

##### The application will be composed of three routes:

  

<li>The first route (the default) renders a form where the user can enter a longer URL to be shortened. On submission, if the form passes validation, then the URL will be shortened. Then, both the original and shortened URLs will be stored in the database.</li>

<li>The second route retrieves an un-shortened URL from a shortened one. If the shortened URL is found in the database the user will be redirected there. If not, then the user will be redirected to the application’s 404 page.</li>

<li>The third route is the application’s 404 page.</li>
<hr>
<br/>
 <b>Note:
This app will contain two classes: a URL shortener service (UrlShortenerService) and a database persistence service (UrlShortenerDatabaseService). The application only directly interacts with the URL shortener service, as that service contains the database persistence service, a member variable, which handles database interaction.
