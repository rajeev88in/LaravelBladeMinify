# LaravelBladeMinify
Minifies Laravel Blade File with HTML, CSS and JQuery on runtime.

<h2 align="left">Steps to Follow: </h2>

 1. Create a Middleware: **MinifyBlade**
 2. Copy the Code from the php file provided.
 3. Register the Middleware to **Kernel.php** under 
    `protected $middlewareAliases `
as
    `'bladeMinify' => \App\Http\Middleware\MinifyBlade::class,` 
	
 at the last line.
 
 4. Copy all the routes under this route. as 

    `Route::middleware(['bladeMinify'])->group(static function ()
    {  
    //Your Routes Here..............
      });`

