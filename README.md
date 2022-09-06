# Code Capsules Express project demo


<a href="https://codecapsules.io/slack">
<img src="https://img.shields.io/badge/join%20slack-%23Code--Capsules-brightgreen"></a>

<br>

<p>
<img src="https://raw.githubusercontent.com/codecaps/demo-express-js/master/static/img/logo-code-capsule-primary.svg" width="100" style="margin-right: 2rem; margin-left:2rem">
<img src="https://raw.githubusercontent.com/codecapsules-io/demo-express-js/master/static/img/express.png" width="100">
</p>

----

Code Capsules is a cloud abstraction tool that allows you 
to build and run apps across clouds. Code Capsules is all about the developer experience. It focuses on getting up and running quickly while still providing the full force and scalability of the cloud. Without locking you into a single cloud provider or region.

**[Check out Code Capsules here][codecapsules]**, 

visit our [docs]

or join the [slack community][slack] <img width="15" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/slack/slack-original.svg" />


----

## Express Demo application

The purpose of this repo is to provide a Node.js code base that is used to test the backend capsule available on Code capsules. The capsule will build the code and then deploy it with a domain (capsule-name.codecapsules.io) that is secure and SSL enabled. You are able to select the performance and scaling while creating the capsule.


### To get started with this app on Code Capsules

- Fork this repo to your git account
- On Code Capsules, from within a team and space (A personal team and space should be set up if you haven't made any yet)
- Create a new capsule
- Select **backend capsule** as the capsule type
- Select the plan to use for the capsule performance and scale.
  - Or select custom plan and set the performance as required.
- Select the repo to use in the capsule (the forked repo)
  - You may need to link this repo specifically if you haven't enabled all repos through git.
  - You can do this with the **Install or Configure Codecapsules on Git** button.
- Leave the remaining fields blank, and press **Create Capsule**


Code capsules directs traffic to port 3000 by default. It can be configured in the capsule detail page once it's been created.

### Listening on `$HOST:$PORT`
The capsule will be supplied with two Environment Variables during runtime:
- **PORT**
  - `3000` by default
  - The port on which traffic will be directed on the capsule. 
- **HOST**
  - `0.0.0.0` by default
  - The IP address that your application should bind to receive traffic.
  - It should be noted that binding to `localhost` may not work.

Frameworks usually provide documentation on how to use an environment variable to get the PORT and HOST values to listen and bind to.

[Here is a resource for Express.js][expressenvvars]

---

## Support

If you need support, start with the [frequently asked questions], 

If you can't find your issue there then reach out to us on [slack] <img width="15" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/slack/slack-original.svg" />


---

[codecapsules]: https://codecapsules.io
[expressenvvars]: https://medium.com/geekculture/node-js-environment-variables-setting-node-app-for-multiple-environments-51351b51c7cd
[docs]: https://codecapsules.io/docs/
[frequently asked questions]: https://codecapsules.io/docs/FAQ/teams-spaces-capsules/
[reference]: https://codecapsules.io/docs/reference/
[slack]: https://codecapsules.io/slack
[blog]: https://codecapsules.io/blog/
[hack days]: https://codecapsules.io/docs/community/codecapsules-hack-days/
