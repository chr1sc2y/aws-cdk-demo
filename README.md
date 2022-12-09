# AWS CDK Demo

## Prerequisit

1. [Install Node.JS](https://nodejs.org/en/)
2. [Create an IAM User](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_users_create.html)
3. [Install AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)
4. [Install AWS CDK Toolkit](https://docs.aws.amazon.com/cdk/v2/guide/cli.html)
5. Prepare your favorite IDE or [AWS Cloud9](https://aws.amazon.com/cn/cloud9/)

## Project Structure

- *lib/\*.ts*: CDK application’s main stack definition.
- *bin/cdk-workshop.ts*: the entrypoint of the CDK application.
- *cdk.json*: tells the toolkit how to run your app. In our case it will be "npx ts-node bin/cdk-workshop.ts"
- *tsconfig.json*: the project’s typescript configuration
- *package.json*: npm module manifest. It includes information like the name of the app, version, dependencies and build scripts like “watch” and “build”
- *package-lock.json*: generated by npm. It describes the exact tree that was generated to allow subsequent installs to have the identical tree.
- *node_modules*: maintained by npm. It includes all the project’s dependencies.

## Useful commands

* `npm run build`   compile typescript to js
* `npm run watch`   watch for changes and compile
* `npm run test`    perform the jest unit tests
* `cdk deploy`      deploy this stack to your default AWS account/region
* `cdk diff`        compare deployed stack with current state
* `cdk synth`       emits the synthesized CloudFormation template
