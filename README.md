# avocado-dashboard
Avocado price and selling dashboard using plotly dash

To run this app on your local machine you need to install the libraries mentioned in the requirements.txt file.
It is recommended to create a new virtual environment for this app and install the dependencies mentioned in the requirements.txt file.

To deploy this app on the cloud, heroku is used.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------

* Firstly, to create the same app on your local machine, you will need app.py, avocado.csv files and assets folder (includes a css file and an image).
  * Copy the code into your local machine run the app.py file.
  * You should be able to run the app on your local machine.

* Follow these steps to deploy it on heroku
  * Install git and heroku cli.
  * Follow this link to download [git](https://git-scm.com/downloads)
  * Follow instructions on this page to install [heroku cli](https://devcenter.heroku.com/articles/getting-started-with-python#set-up) and login to heroku from cli by typing `heroku login` in the terminal.

* After that create two more files Procfile and runtime.txt.
  * Copy the content of Procfile and runtime.txt from this repo into your local machine.
* For requirements.txt, type `pip freeze > requirements.txt` into your project's root directory. It will create a requirements.txt file with all the dependencies and its versions.

* Now initialize your local repo using `git init`.
* Create a .gitignore file and add your virtual environment folder into it (We dont want to track the changes made in the virtual environemnt folder).
* Type `git add .` It tells git that you want to include updates to all the files in the next commit.
* Type `git commit -m 'your commit message'` this command captures a snapshot of the project's currently staged changes.

* Now, we need to create an app in heroku for that use `heroku create YOUR-APP-NAME`.
* After that we push the code to heroku master using `git push heroku master`.

Our app is deployed on heroku.

Final app will look like [this](https://klaptor-avocado-dashboard.herokuapp.com/)
