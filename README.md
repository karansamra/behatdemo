# behatdemo
BDD PHP framework Behat Implementation by Jsingh7[Jaskaran]

1. Run composer install command from the root directory so that it can download all the dependancies.
	
	sudo php composer.phar install
	
2. Run init command to initailise behat from the root of the project. It will create your feature directory.
	
	vendor/bin/behat --init
	
3. You can create feature files in features directory.
	
	for e.g. test.feature
	
4. If you want to use prebuilt context functions you may use MinkContext class. 
	As we have defined mink package in our dependancies so we can directly use it in our FeatureContext.php
	
	use Behat\MinkExtension\Context\MinkContext;

5. To perform tests using web-browser you need "Selenium-server stand alone jar file", 
	it can live anywhere on your computer.
	Add selenium2 driver in your behat.yml
	
	selenium2: ~
	
	Now you can add @javascipt tag above your senarios and it will use web-browser to perform tests.
	