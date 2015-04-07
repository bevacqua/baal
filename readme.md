# baal

> Automated, autoscaled, zero-downtime, immutable deployments using plain old bash, Packer, nginx, Node.js, and AWS. Made easy.

Read about this deployment strategy on [Pony Foo][1], and then clone this repository. Copy the scripts, and adjust as needed. A few pointers.

- The application is named `baal` in a few places. Change that to your application's name
- You need to set a value for `HOSTED_ZONE` in the `setup` script. Read the articles on [Pony Foo][1] to learn about that
- In the `deploy` script you can set `PRIMAL_ID` to an AMI so that your base AMI isn't rebuilt on every deploy
- By default, `baal` expects to build your static assets with `npm run build-$NODE_ENV`

Relevant [Pony Foo][1] articles:

- [Immutable Deployments and Packer][2]
- [Leveraging Immutable Deployments][3]

# license

MIT

[1]: http://ponyfoo.com
[2]: http://ponyfoo.com/articles/immutable-deployments-packer
[3]: http://ponyfoo.com/articles/leveraging-immutable-deployments
