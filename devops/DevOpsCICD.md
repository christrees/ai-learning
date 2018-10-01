# DevOps Foundations


## Continuous Integrations and Continuous Deliver
1. DevOps core concept: CI/CD
2. Benifits
3. Build pipelines in practice

## Build your Pipeline

1. Github
2. Jenkins

## Resources
+ https://github.com/wickett/continuous-delivery-class
+ https://github.com/wickett/word-cloud-generator
+ https://theagileadmin.com/what-is-devops/

## Detail

Following along with the demos
- [Narrator 1] First couple words on Following Along With The Demos. So with the sample files, we've provided a readme.md file that contains a lot of information on how to setup your system for each individual step. The biggest one that you'll want to do is to install Docker for Mac/Windows or other from Docker.com so that you can run the Jenkins and Nexus, and test fixture containers. - [Narrator 2] Reversion control in action we install Homebrew.
With that we install Go, Vim, and Git. There's also some setup for how you setup your path for working with Go. - [Narrator 1] You'll also need a Github account, with your appropriate SSH keys installed to be able to pull the Word Cloud Generator App. - [Narrator 2] For the CIN action with Jenkins video and the following videos you'll need Docker installed as mentioned. The ReadMe contains the information seen in the video on how to start and how to stop it. - [Narrator 1] For the video on Unit Testing in Action many of the same requirements we setup earlier for Git are the same here but again, you want to make sure you have Go installed, Vim, Git, and a lot of the profile settings for Go in your Go path.
- [Narrator 2] For Deployment in Action with Chef all of the installation has already been performed as part of the Docker Containers provided but the ReadMe contains information on how to run it by hand if you'd like to. For Integration in Testing in Action with abao this container is also built by the Docker Compose File but if you want to build it by hand and run it with or without a Hook File the instructions are here on how to do that. For UI Testing in Action with Robot, as I mentioned during that course it's possible that the virtual end provided might end up not working on your system.
If that's the case you can just blow away that VENV directory inside the Robot Test subdirectory and execute this sequence of commands. Essentially you're installing the Viretualenv Python Package. You're installing a bunch of stuff in it and then when you're done you deactivate out of that VENV. And then anytime you want to run it, you go into Robot Tests, you source that Activate Script, you run Robot and then of course eventually you'd deactivate again whenever you want to get out of it.
- [Narrator 1] For doing Security Testing in Action with Gauntlt again we use Homebrew, also Docker again for Mac but we also use retire.js and that's a node package installed via NPM. Sort of a couple of other requirements here as well. Because the way Gauntlt talks to Arakney, there's a setting in their Esty Host File to set local host 127.0.0.1 over to a name Word Cloud. - [Narrator 2] So there's a couple advanced topics in case you have problems.
So the Jenkins Docker container itself runs a Docker container to run abao the Integration Testing. If you get an error of this form about permission denied when trying to connect to docker.sock, the solution I have in here it works for Mac for sure. You may need to determine the actual ownership of the Var Run Docker Sock File on your system and in the Docker File for CD Jenkins, change the line that does an ownership change specifically.
On Mac it's owned by Staff, on Lenux it's often owner by Docker. And whatever you would need to do on you flavor of Windows system to make that actually work. There's also some information in here on running the containers in isolation if you don't want to play with them without using the Docker Compose File and some information on if you're going to start from scratch instead of using our provided Jenkins Home and Nexus home directories.
How you can go through a little bit of that setup on your own. And then finally the Test Fixture. I had mentioned that I had setup some of the Chef Cookbook Skeletons and what not. I didn't want that to be totally magic so that is also here in the ReadMe and you can start you know, with an empty directory and set all this up on your own for an additional learning festive experience. - [Narrator 1] Alright, well we hope you enjoy the course and thanks for tuning in.
