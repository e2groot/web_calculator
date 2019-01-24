# web_calculator
Simple web calculator accessible over HTTP.

This calculator was an example I followed to further understand Kotlin and how it works with DropWizard.
Unit tests will eventually be added, but this was just to try it out for my interest and curiosity.
I took it a little further to learn how to encapsulate this as a Docker image and run as a container.



The image of this runnable application can be found here:
  https://hub.docker.com/r/e2groot/web-calculator-image

Test the application by running the commands:

#15 should be the answer

curl "localhost:8080/add?a=5&b=10"




#50 should be the answer

curl "localhost:8080/multiply?a=5&b=10"
