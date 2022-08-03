# Spinnaker

spinnaker is a multi-cloud continuous delivery platform that supports releasing and deploying software changes across different cloud providers, including AWS EC2, Kubernetes, Google Compute Engine, Google Kubernetes Engine, Google App Engine, etc.

Spinnaker key features:

* Creates deployment pipelines that run integration and system tests, spin up and down server groups, and monitor rollouts. Trigger pipelines via Git events, Jenkins, Travis CI, Docker, cron, or other Spinnaker pipelines
 * Create and deploy immutable images for faster rollouts, easier rollbacks, and the elimination of hard to debug configuration drift issues
* Tie your releases to monitoring services such as Datadog, Prometheus, Stackdriver, or SignalFx, using their metrics for canary analysis
* Install, configure, and update your Spinnaker instances with Halyard – Spinnaker’s CLI administration tool
* Set up event notifications for email, Slack, HipChat, or SMS (via Twilio)

## Spinnaker vs Jenkins 
The key differences between Spinnaker vs Jenkins are as follows:

* The first and foremost difference is that users think that Spinnaker is a build tool, but the truth is it’s not a build tool; in fact, it can be integrated with build tools like Jenkins.
* To deploy AWS Amazon Web Services in your project, Spinnaker API is used in Jenkins jobs.
* For releasing software, Jenkins is used for continuous integration in the development process, which helps maintain everything online with ease through one master server.
* For releasing software, Spinnaker is used for continuous delivery in the development process, which helps in maintaining everything online such as starting jobs and monitoring progress in the process.
* Spinnaker was introduced in the market to combine Continuous Integration (CI) and Continuous Delivery (CD) together.
* Spinnaker is designed for cloud deployment purposes, whereas Jenkins isn’t. Therefore, for implementing cloud deployment in Jenkins, you have to write the external script in the pipeline scripting manually.
* Spinnaker is an open-source continuous delivery platform for cloud-based enterprises’ deployment at a small and large scale, whereas Jenkins is usually suitable for smaller divisions.
* If you are working with Jenkins and you want to make your deployment phase faster and flexible, then spinnaker can be used for that purpose.
* You can have a complete dashboard in Spinnaker with features including resource management and multiple cloud environments, whereas Jenkins has no such dashboard, but with the help of plugins, this feature can be implemented.
* The pipeline feature in Spinnaker is cloud-centered for continuous delivery, whereas the Jenkins pipeline feature is server-centered for continuous integration purposes.
* Jenkins performs better than Spinnaker when the task is related to running multiple test cases, building packages for classes and, most important, SCM (Source Control Management).

\*taken from https://www.educba.com/spinnaker-vs-jenkins/

From reading evaluations it suggust they have their own areas of strength and could be used together: Jenkins to manage CI, and Spinnaker, which integrates seamlessly with Jenkins, for CD.

# Set up
Instuctions are documented here: https://spinnaker.io/docs/setup/
I chose to try the "Try it Out quick start solutuion which pointed to this Spinnaker All-In-One (Minnaker) Project https://github.com/armory/minnaker

## My experience
* Didnt manage to get it working in the allotted time due to trying to set up my system. the instructions suggested setting it up in a VM; 
* Couldnt get VM working my my linux machine (think I needed to adjust the BIOs) - didnt want to play around with that
* decide to try running up an Ubuntu Docker image to do this in which resulted in having to set alot of addtional setting/packages etc.

## Full installation 
There's 


## Prereqs
1. A machine on which to install Halyard
2. A Kubernetes cluster on which to install Spinnaker itself

## Installing a complete Spinnaker involves these steps:

1. Install Halyard
2.  Choose a cloud provider
3. Choose an environment
4. Choose a storage service
5. Deploy Spinnaker
6. Back up your config
7. Configure everything else (which includes a lot of stuff you need before you can use Spinnaker in production)
8. Productionize Spinnaker (which mainly helps you configure Spinnaker to scale for production)
 
