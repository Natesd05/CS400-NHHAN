run: App.class
	java App

Mercury:
	@echo Hello Mercury

App.class: App.java
	javac App.java

test: App.class TestApp.class
	java -jar ../junit5.jar --class-path=. --select-class=TestApp

TestApp.class: App.class TestApp.java
	javac -cp .:../junit5.jar TestApp.java 