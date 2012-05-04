Github Pull Request Validator
==============

A tool for automatically validating github pull requests with Jenkins



Configuring
-----------

Here's an example `ghpr.conf` file.

    scala: {
      jenkins: {
        url = "https://my.company.com/jenkins"
        user: {
          user = "buildbot"
          password = "MY PASSWORD IS SECRET"
        }
        jobs: [ "flush-silly-mistakes" ]
      }
      github: {
        user: {
          user = "gh-commenter"
          password = "MY PASSWORD IS SECRET"
        }
        project: {
          user = "myname"
          project = "myproject"
        }
      }
    }



Contributing
------------
If you'd like to contribute to the GHPRValidator project, please sign the [contributor's licensing agreement](http://www.typesafe.com/contribute/cla).

License
-------
Copyright 2012 Typesafe, Inc.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   [http://www.apache.org/licenses/LICENSE-2.0](http://www.apache.org/licenses/LICENSE-2.0)

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
