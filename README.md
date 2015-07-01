sample_ubuntu1204_go
====================

This sample helps you create a shippable.yml file for your go project on Shippable. Please refer to our [language specific documentation on go](http://docs.shippable.com/languages/#go) for more details.

### Build Image

The sample uses a go specific build image that's available for public use:
 [shippableimages/ubuntu1204_go](https://registry.hub.docker.com/u/shippableimages/ubuntu1204_go)  ([Dockerfile](https://github.com/shippableImages/ubuntu1204_go/blob/master/Dockerfile)).

The testing framework used here is [Ginkgo](http://onsi.github.io/ginkgo/)

To set your build image in Shippable:
- Login to [Shippable](https://www.shippable.com) 
- Navigate to your project page by clicking on the project link
- Click on **Settings** and choose the following option:

`Pull Image from : shippableimages/ubuntu1204_go`

The go versions available in these images are:

- 1.1
- 1.2
- 1.3
- tip
- release
 
Activate gvm in before_install section to run your build against the correct version of go.

For more details on project settings, you can refer our docs on  [Build and Project Settings](http://docs.shippable.com/project_settings).
