# Simple QuickStart

This quickstart runs a Java application using a main class.

This example is implemented using very simple Java code.
The source code is provided in the following java file `src/main/java/io/fabric8/quickstarts/java/simple/Main.java`,
which can be viewed from [github](https://github.com/fabric8io/ipaas-quickstarts/blob/master/quickstart/java/simple-mainclass/src/main/java/io/fabric8/quickstarts/java/simple/Main.java).

This example is printing *Hello Fabric8! Here's your random string: lRaNR* to the standard output in the infinite loop.


### Building

Navigate to the `java-mainclass' folder and the example can be built with

    mvn clean install


### Running the example locally

The example can be run locally using the following Maven goal:

    mvn exec:java


### Running the example on Kubernetes or OPenShift

It is assumed a running Kubernetes platform is already running. If not you can find details how to [get started](http://fabric8.io/guide/getStarted/index.html).

    mvn fabric8:run
    
To list all the running pods in Kubernetes type:

    kubetl get pods

Or on OpenShift type:

    oc get pods

Then find the name of the pod that runs this quickstart, and output the logs from the running pods with:

    kubectl logs <name of pod>

You can also use the fabric8 [web console](http://fabric8.io/guide/console.html) to manage the running pods, and view logs and much more.


### More details

You can find more details about running this [quickstart](http://fabric8.io/guide/quickstarts/running.html) on the website.

