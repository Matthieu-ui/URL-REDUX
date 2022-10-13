# url4short

URL shortener with PHP and PostgreSQL

  

# The application will be composed of three routes:

  

<li>The first route (the default) renders a form where the user can enter a longer URL to be shortened. On submission, if the form passes validation, then the URL will be shortened. Then, both the original and shortened URLs will be stored in the database.</li>

<li>The second route retrieves an un-shortened URL from a shortened one. If the shortened URL is found in the database the user will be redirected there. If not, then the user will be redirected to the application’s 404 page.</li>

<li>The third route is the application’s 404 page.</li>

 <b>Note:
This app will contain two classes: a URL shortener service (UrlShortenerService) and a database persistence service (UrlShortenerDatabaseService). The application only directly interacts with the URL shortener service, as that service contains the database persistence service, a member variable, which handles database interaction.

 # Required PHP dependencies
| Dependency    | Description |
| -------- | ------- |
| laminas/laminas-db | laminas-db provides a database abstraction layer, and SQL abstraction implementations.   |
| laminas/laminas-diactoros | laminas-diactoros provides an implementation of PSR (PHP Standard Recommendation) HTTP Messages. Included because custom response classes are an intuitive way of returning responses from requests. |
| laminas/laminas-inputfilter | laminas-inputfilter filters and validates data from a range of sources, including files, user input, and APIs. |
  | laminas/laminas-uri | laminas-uri helps with manipulating and validating URIs (Uniform Resource Identifiers). |
  | php-di/slim-bridge | Slim Bridge integrates PHP-DI, an excellent dependency injection (DI) container, with Slim. |
  | slim/slim | This is the core of the Slim micro framework |
  | slim/psr7 | This library integrates PSR-7 into the application. It's not strictly necessary, but I feel it makes the application more maintainable and portable.|
  | slim/twig-view	 | This package integrates the Twig templating engine making it easier to create response bodies.|
  | vlucas/phpdotenv	 | PHP dotenv helps keep sensitive configuration details out of the code (and version control).|
  
