# Ruby sample for 23's Visualplatform API

This is a sample on how to authenticate your application for and integration it with 23's Visualplatform API available at http://community.23video.com/api/.

The sample is available through...

* [API documentation and samples on Github](http://github.com/23/DeveloperDocumentation)
* [All ruby sample scripts](http://github.com/23/DeveloperDocumentation/tree/master/lib/ruby/)



## Requirements

These scripts require Ruby and for the following Ruby gems to be installed:

    oauth
    mime
    mime-types
    yaml


## Authentication

The API uses an OAuth-based authentication scheme for granting application access and for signing request. See [oauth.net](http://oauth.net) for further details.

To prepare authentication, first following the documented steps to set up a consumer key and a consumer secret with 23, and then run the following command.

    visualplatform-authenticate.rb -k <consumer_key> -s <consumer_secret> 

After you've completed the step prescribed in the script, you'll find a new file (`oauth.yml`) in your working directory containing your secret credentials -- including an access key and an access token.


## Usage

After authenticating your application, you can invoke an API method from the command-line by running:

    visualplatform-command.rb <api_method> <param1> <value1> <param2> <value2> ...

For example

    ./visualplatform-command.rb /api/echo iam here title "My title"


This sample also shows how to build multipart requests and upload files to 23 Video through Ruby.
