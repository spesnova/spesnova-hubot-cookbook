# Description
This cookbook is designed to deploy the hubot instance.
Using cookbook library/application pattern.

Todo:

* Install Nodejs
* Determine how do manage hubot script
* logrotate?

# Requirements

* hubot (opscode)

# Usage
Include the recipe on your node or role that fits how you wish to install Kandan on your system per the recipes section above. Modify the attributes as required in your role to change how various configuration is applied per the attributes section above. In general, override attributes in the role should be used when changing attributes.

# Attributes

* `node["hubot"]["version"]` - The hubot version
* `node["hubot"]["script_version"]` - The hubot script version
* `node["hubot"]["install_dir"` - The path to deploy hubot.
* `node["hubot"]["user"]` - The user to install and run the hubot.
* `node["hubot"]["group"]` - The group to install and run the hubot.
* `node["hubot"]["name"]` - Alias name in chat for the hubot.
* `node["hubot"]["adapter"]` - The hubot adapter you use.
* `node["hubot"]["dependencies"]` - The dependency npm packages. Hash
* `node["hubot"]["config"]` - The config about the hubot. Hash

# Recipes
## spesnova-hubot::default
This recipe deploy a hubot instance.

# Author

Author:: Seigo Uchida (<spesnova@gmail.com>)

Copyright:: 2013 Seigo Uchida (<spesnova@gmail.com>)

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

```
http://www.apache.org/licenses/LICENSE-2.0
```

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.