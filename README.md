## Resin Golang Image Example

This project contains examples of how to use Resin Golang images on devices supported by [resin.io][resin-link]. All details about Resin Golang images can be found [here][base-images].

There are two examples in this project. You can select the example by editing `start.sh` script.

To get this project up and running, you will need to signup for a resin.io account [here][signup-page] and set up a device, have a look at our [Getting Started tutorial][gettingStarted-link]. Once you are set up with resin.io, you will need to clone this repo locally:

Then add your resin.io application's remote:
```
$ git remote add resin username@git.resin.io:username/myapp.git
```
and push the code to the newly added remote. To push the code to ARM boards, we need to select native ARM builders for the build by doing:
```
$ git push resin master:master-arm
```
To push the code to other platforms, we do:
```
$ git push resin master
```
It should take a few minutes for the code to push. While you wait, lets enable device URLs so we can see the server outside of our local network (outyet example needs this). This option can be found in the `Actions` tab in your device dashboard.

[resin-link]:https://resin.io/
[signup-page]:https://dashboard.resin.io/signup
[gettingStarted-link]:http://docs.resin.io/#/pages/installing/gettingStarted.md
[base-images]:http://docs.resin.io/#/pages/runtime/resin-base-images.md
