This projects uses repository pattern which is a good practice for some developers. 
According to my experience and research, Laravel community does not support this pattern too much. 
Laravel itself doeesn't have any documentation or Laravel has not highlighted anywhere of using this pattern.
Either I would suggest to use traits or helper functions to achive this approch as it is suggested by Laravel.
I believe that when using any framework we should take 100% benefits of it and we should try to use what the framework suggests. 

The worst part is that I can see that laravel's validation system is not used at all, rather conditions are manually added.
Also there is a lot of code in controllers, controllers should always be concised and all the logic should be moved from controlers.
There should be scopes defined in models so instead of where clauses we should use scopes.


TO change the status of jobs there are multiple functions defined. this should be done either in update function OR there should be only 1 function to update the status. 