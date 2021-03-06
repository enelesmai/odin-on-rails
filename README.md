# odin_on_rails

How to start a rails application guided by Odin Project, following git-flow and deployed to heroku.


## Built With

* Ruby 2.6.5
* Rails 5.2.4
* VSCode


## Getting Started

The project was designed to create an scaffolded application with rails, following git-flow practices and deploying to heroku.

If you want to deploy this application to your heroku account follow the instructions in this [link](https://www.theodinproject.com/courses/ruby-on-rails/lessons/your-first-rails-application-ruby-on-rails#step-3-deploy-your-rails-application).

**You need to know**

1. After `heroku create` you may need to add heroku as a remote source, use the following command:

    git remote add local-branch-name https://git.heroku.com/remote-app-123.git
    
    or

    heroku git:remote -a remote-app-123

Do this **only if you don't see** `heroku` in the output of the command `git remote` on your terminal. Visit [Deploying with Git](https://devcenter.heroku.com/articles/git) for more information.

2. Heroku is by default working only with code commited to master, but there is a way to [force it to take your non master branch](https://stackoverflow.com/questions/14593538/make-heroku-run-non-master-git-branch). You can type:

    git push link-heroku-app local-branch:master

For more information on how to deploy to heroku visit the official [Heroku documentation](https://devcenter.heroku.com/articles/getting-started-with-rails4#local-workstation-setup).

As an example, where *https://git.heroku.com/afternoon-caverns-32087.git* is the remote heroku repo and *rails-app* is your current branch, the next command should be typed to succesfully push to heroku:

    git push https://git.heroku.com/afternoon-caverns-32087.git rails-app:master

3. Finally, before pushing to heroku remember to [remove *.bundle*](https://forum.theodinproject.com/t/having-an-issue-with-git-push-heroku-master/30575) folder so Heroku will create its own bundle when you push your code there, this is for fixing an issue like [this one](https://stackoverflow.com/questions/12333224/hartls-chapter-7-when-pushing-to-heroku-pg-is-not-part-of-the-bundle-but-it).


**Running the program on local machine**

Clone the repository to your local machine.
To install gems run

    bundle install
       
then run the server on https://localhost:3000

    rails server 



## Live Demo
![image](https://user-images.githubusercontent.com/5160907/79511012-10e6b100-8004-11ea-9746-8d0a2f0837b8.png)

Visit the live demo [here](https://afternoon-caverns-32087.herokuapp.com/).


## Author

👤 **Xóchitl Selene Flores Pérez**

- Github: [@enelesmai](https://github.com/enelesmai)
- Twitter: [@enelesmai](https://twitter.com/enelesmai)
- Linkedin: [xochitlselene](https://linkedin.com/in/xochitlselene)


## 🤝 Contributing

Contributions, issues and feature requests are welcome!

Feel free to check the [issues](https://github.com/enelesmai/odin_on_rails/issues).


## Show your support

Give a ⭐️ if you like this project!
