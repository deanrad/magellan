Installing the Magellan rails plugin gives you a controller that lets you explore and evaluate values inside your ruby process.

* Install it to vendor plugins 

    git submodule add 'git://github.com/chicagogrooves/magellan.git' vendor/plugins/magellan

* Add the following to config/environments/development.rb

    ENV["MAGELLAN_ON"]="1"

The magellan controller class IS NOT EVEN DEFINED unless this variable is set.
The combination of this fact it will not be leaked into a production environment. It is NOT suggested that magellan be enabled in a production environment !
  
* Go to this URL to interact with your running server process.

    http://localhost:3000/magellan/console

* Toggle the ability to attach a debugger like ruby-debug into the process (NOT IMPLEMENTED YET)

* Initiate an attachment from your editor/IDE to do remote debugging (NOT IMPLEMENTED YET)
