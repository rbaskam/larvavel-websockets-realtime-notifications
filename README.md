
## Tutorial
Find the tutorial at https://robert-askam.co.uk/posts/creating-real-time-notifications-in-laravel-with-laravel-web-sockets

To start run php artisan websockets:serve
Go to http://localhost:8000/laravel-websockets and click connect to see notifications
Then php -S localhost:8000 -t public

Import DB

Open Tinker
Make sure you have a user
$user = User::first();
Then:
$user->notify(new App\Notifications\RealTimeNotification('Hello World'));

Check your console in the home page of your laravel add.