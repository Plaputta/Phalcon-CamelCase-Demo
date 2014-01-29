Results in Phalcon 1.2.3:

The view for 'indexAction' in 'IndexController' is located at '/apps/frontend/views/index/index.phtml'

Try /awesome-test/super-action, it will call action 'mySuperTestAction' in 'MyAwesomeTestController' and load the view '/apps/frontend/views/my_awesome_test/mysupertest.phtml'.

But if you try /i-do-not-exist, it will fall back to action 'pageNotFoundAction' in 'ErrorController' and load the view '/apps/frontend/views/Error/pageNotFound.phtml'.

Results in Phalcon 1.2.6:

The view for 'indexAction' in 'IndexController' is located at '/apps/frontend/views/Index/index.phtml'

Try /awesome-test/super-action, it will call action 'mySuperTestAction' in 'MyAwesomeTestController' and load the view '/apps/frontend/views/myAwesomeTest/mysupertest.phtml'.

But if you try /i-do-not-exist, it will fall back to action 'pageNotFoundAction' in 'ErrorController' and load the view '/apps/frontend/views/Error/pageNotFound.phtml'.

You can watch the headers 'X-Action' and 'X-Controller' to see what's the output of the 'beforeDispatch' event.
