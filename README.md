REQUISITOS

WIINDWOWS 

IDE VSCODE

JDK 11
JRE 1.8
MAVEN 3.8.6

Comando para relaizar la pruena y levantar srenity
nvm verify

SE ADJUNTA CAPTURAS ARHCIVO .doc


EJERCICIO:
Realizar una prueba funcional automatizada (Prueba E2E) de un flujo de compra en la página
http://opencart.abstracta.us/ que incluya:
• Agregar dos productos al carrito
• Visualizar el carrito
• Completar el “Checkout” como invitado: “Guest Checkout”
• Finalizar la compra hasta la confirmación: “Your order has been placed!”

README
SERENITY WEB TRAINING

Install skipping the tests:
mvn install -DskipTests

Run the tests:
GRADLE
gradle clean test -Dwebdriver.driver=firefox -Denvironment=staging
gradle clean test -Dwebdriver.driver=chrome -Denvironment=staging

MAVEN
mvn clean verify -Dwebdriver.driver=chrome -Denvironment=staging



Running by tags

Maven:
mvn verify -Dcucumber.options="--tags '@login or @foo'"
mvn verify -Dcucumber.options="--tags @login"


gradle clean test -Dcucumber.options="--tags '@login or @foo'"
gradle clean test -Dcucumber.options="--tags @login"

CHROME PREFERENCES:

https://johnfergusonsmart.com/configuring-chromedriver-easily-with-serenity-bdd/
https://chromium.googlesource.com/chromium/src/+/master/chrome/common/pref_names.cc


