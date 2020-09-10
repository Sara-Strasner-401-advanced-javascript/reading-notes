# Heroku
Heroku is a platform as a service (PaaS) that enables developers to build, run, and operate applications entirely in the cloud. Developers use Heroku to deploy, manage, and scale modern apps. 

The Heroku Command Line Interface (CLI) utilizes Git. You use the CLI to manage and scale your applications, provision add-ons, view your application logs, and run your application locally.

`heroku create` creates an app on Heroku, which prepares Heroku to receive your source code.

When you create an app, a git remote (called heroku) is also created and associated with your local git repository.

`git push heroku main` deploys your code.

You can visit your newly deployed app via `heroku open`

View logs
Heroku treats logs as streams of time-ordered events aggregated from the output streams of all your app and Heroku components, providing a single channel for all of the events.

View information about your running app using one of the logging commands, `heroku logs --tail`

Press Control+C to stop streaming the logs.
