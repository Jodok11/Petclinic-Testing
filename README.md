# Petclinic-Testing

How To Setup:
Clone the following two GitHub Repositories into the same directory:
https://github.com/spring-petclinic/spring-petclinic-angular
https://github.com/Jodok11/spring-petclinic-rest

Setup and Run the Angular and Rest Projects according to their descriptions.
Then, open your choice of JAVA IDE (I used IntelliJ) and navigate to the "test" Directory, in there to java and then the sub-folder(s), until you hit 'petclinic'.
There, simply right-click on the "e2e" Folder and select "Run Tests in e2e". This then executes all the Tests I have written automatically.
Side-note, mvn test would also be an option, but there was some trouble with the Frontend Tests, namely Selenium, which is why I chose the method above.
Since the Chromedrive is in the Rest Repo, that should all work normally, but based on your Browser that could pose a problem. Please then check your Browser Version and install an according Driver.
Frontend Tests do not have Cleanup in them (due to time reasons), therefore re-start the Rest service when you want to re-do those tests. 
If FE Tests fail, try to rerun them manually in the IDE. (Selenium sometimes behaves weirdly / the Code doesnt wait for a page to load or stuff like that)

Test reporting would be viewable via mvn allure:serve after mvn test, but I could not finish integrating them, so for now the Reporting is missing.

If there are any Questions, feel free to reach out to me. 
