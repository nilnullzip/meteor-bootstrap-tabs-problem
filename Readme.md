###Demo of a problem with Meteor/Iron-router and Bootstrap tabs. 

When operating correctly, the URL in the address bar should follow the tab being selected. When operating incorrectly, the URL does not change at all. The difference between the demo working or not depends on the order of iron-router and bootstrap in .meteor/packages.

The repository is configured for the working case. Just edit the packages file to the failing case and restart meteor to see it fail.

#### Working case

> http://meteor-bootstrap-tab-problem-good.meteor.com

with this packages file:

	standard-app-packages
	preserve-inputs
	iron-router
	bootstrap
	accounts-ui
	accounts-password
	showdown
	underscore

#### Failing case

> http://meteor-bootstrap-tab-problem-bad.meteor.com

with this packages file:

	standard-app-packages
	preserve-inputs
	bootstrap
	iron-router
	accounts-ui
	accounts-password
	showdown
	underscore

