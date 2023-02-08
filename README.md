# multi-deploy
a sandbox for fun, profit and enjoyment from correcting things while learning Dev---Ops
## Credits
This repo wouldn't have been possible without the touch of
[https://github.com/stephengrinder/Docker-react](https://github.com/stephengrinder/Docker-react)
The code in the repo is his and based upon the following
course
[https://www.udemy.com/course/docker-and-kubernetes-the-complete-guide](docker-and-kubernetes-the-complete-guide)

I don't own any code, just attempted to make it a bit more secure by updating the needed images and packages to the best of my limited time and knowledge.
Use the code on your own risk.

## Architecture

- A multi-container deployment in Docker and AWS consisting of:
  - npm test container for running CI tests
  - front-end nginx handling the client requests
  - client part for handling the factoriel calculations
  - server part
  - redis container
  - postgresql container
  - worker container
  - Docker CI github actions running code testing, building and testing the images and finally pushing the needed images to Dockerhub personal account registries.
  - Trivy scan action
  - Sonar cloud
  - ZAP proxy
  - AWS deployment action

  ## Things to improve

  - rework code to scan entire docker repos. Saw some samples, but too pushy to make things work in limited time.
  - use less typing and better actions if possible. Comes with a steep learning curve. Try learning something new while $LIFE haunts you.


