# UpdateHub Yocto Project Reference Platform

To get the platform you need to have `repo` installed and use it as:

Install the `repo` utility:

```shell
$ mkdir ~/bin
$ curl http://commondatastorage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
$ chmod a+x ~/bin/repo
```

Download the platform source:

``` shell
$ PATH=${PATH}:~/bin
$ mkdir updatehub-platform
$ cd updatehub-platform
$ repo init -u https://github.com/UpdateHub/updatehub-yocto-project-reference-platform.git -b dunfell
$ repo sync

```

At the end of the commands you have every metadata you need to start work with.

Setup the environment:

``` shell
$ source ./setup-environment build
```

Build updatehub-image-minimal

``` shell
$ bitbake updatehub-image-minimal
```

## Contributing

UpdateHub is an open source project and we love to receive contributions from our community.
If you would like to contribute, please read our [contributing guide](https://github.com/UpdateHub/updatehub/blob/v1/CONTRIBUTING.md).

## License

UpdateHub Yocto Project Reference Platform is licensed under the MIT License.
See [COPYING.MIT](https://github.com/UpdateHub/updatehub-yocto-project-reference-platform/blob/master/COPYING.MIT) for the full license text.

## Getting in touch

* Reach us on [Gitter](https://gitter.im/UpdateHub/community)
* All source code are in [Github](https://github.com/UpdateHub)
* Email us at [contact@updatehub.io](mailto:contact@updatehub.io)
